# Comparing `tmp/beetcamp-0.9.1.tar.gz` & `tmp/beetcamp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetcamp-0.9.1.tar", last modified: Fri Jun  4 12:41:28 2021, max compression
+gzip compressed data, was "beetcamp-0.9.3.tar", max compression
```

## Comparing `beetcamp-0.9.1.tar` & `beetcamp-0.9.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    18053 2020-12-06 01:46:15.483202 beetcamp-0.9.1/LICENSE
--rw-r--r--   0        0        0     5983 2021-05-20 01:58:56.623839 beetcamp-0.9.1/README.md
--rw-r--r--   0        0        0    11983 2021-06-02 14:22:33.439510 beetcamp-0.9.1/beetsplug/bandcamp/__init__.py
--rw-r--r--   0        0        0    16199 2021-06-04 12:33:36.668997 beetcamp-0.9.1/beetsplug/bandcamp/_metaguru.py
--rw-r--r--   0        0        0      880 2021-06-04 12:39:11.332304 beetcamp-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     6903 2021-06-04 12:41:28.737905 beetcamp-0.9.1/setup.py
--rw-r--r--   0        0        0     6798 2021-06-04 12:41:28.740001 beetcamp-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    18053 2020-12-06 01:46:15.483202 beetcamp-0.9.3/LICENSE
+-rw-r--r--   0        0        0     6166 2021-07-30 05:44:51.072971 beetcamp-0.9.3/README.md
+-rw-r--r--   0        0        0    12401 2021-08-01 00:40:27.220108 beetcamp-0.9.3/beetsplug/bandcamp/__init__.py
+-rw-r--r--   0        0        0    15988 2021-08-01 00:40:27.220108 beetcamp-0.9.3/beetsplug/bandcamp/_metaguru.py
+-rw-r--r--   0        0        0      993 2021-08-01 00:40:27.226774 beetcamp-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     7081 2021-08-01 00:41:30.029651 beetcamp-0.9.3/setup.py
+-rw-r--r--   0        0        0     6969 2021-08-01 00:41:30.031722 beetcamp-0.9.3/PKG-INFO
```

### Comparing `beetcamp-0.9.1/LICENSE` & `beetcamp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beetcamp-0.9.1/README.md` & `beetcamp-0.9.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![image](http://img.shields.io/pypi/v/beetcamp.svg)](https://pypi.python.org/pypi/beetcamp)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=snejus_beets-bandcamp&metric=alert_status)](https://sonarcloud.io/dashboard?id=snejus_beets-bandcamp)
 
 Plug-in for [beets](https://github.com/beetbox/beets) to use Bandcamp as
 an autotagger source.
 
 This is an up-to-date fork of [unrblt/beets-bandcamp](https://github.com/unrblt/beets-bandcamp)
 
 # Installation
```

### Comparing `beetcamp-0.9.1/beetsplug/bandcamp/__init__.py` & `beetcamp-0.9.3/beetsplug/bandcamp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,22 @@
 """Adds bandcamp album search support to the autotagger."""
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import logging
 import re
 from functools import partial
 from html import unescape
-from operator import attrgetter, truth
+from operator import truth
 from typing import Any, Callable, Dict, Iterator, List, Optional, Sequence, Set, Union
 
-import beets
-import beets.ui
-import beetsplug.fetchart as fetchart
 import requests
 import six
-from beets import plugins
-from beets.autotag.hooks import AlbumInfo, Distance, TrackInfo
-from beets.library import Item
+from beets import __version__, config, library, plugins
+from beets.autotag.hooks import AlbumInfo, TrackInfo
+from beetsplug import fetchart
 
 from ._metaguru import DATA_SOURCE, DEFAULT_MEDIA, Metaguru, urlify
 
 JSONDict = Dict[str, Any]
 
 DEFAULT_CONFIG: JSONDict = {
     "preferred_media": DEFAULT_MEDIA,
@@ -45,15 +42,15 @@
     "art": False,
     "exclude_extra_fields": [],
 }
 
 SEARCH_URL = "https://bandcamp.com/search?q={0}&page={1}"
 ALBUM_URL_IN_TRACK = re.compile(r'inAlbum":{[^}]*"@id":"([^"]*)"')
 SEARCH_ITEM_PAT = 'href="(https://[^/]*/{}/[^?]*)'
-USER_AGENT = "beets/{} +http://beets.radbox.org/".format(beets.__version__)
+USER_AGENT = "beets/{} +http://beets.radbox.org/".format(__version__)
 ALBUM_SEARCH = "album"
 ARTIST_SEARCH = "band"
 TRACK_SEARCH = "track"
 
 ADDITIONAL_DATA_MAP: Dict[str, str] = {
     "lyrics": "lyrics",
     "description": "comments",
@@ -82,15 +79,16 @@
             return ""
         return unescape(response.text)
 
 
 class BandcampAlbumArt(BandcampRequestsHandler, fetchart.RemoteArtSource):
     NAME = "Bandcamp"
 
-    def get(self, album: AlbumInfo, plugin, paths) -> Iterator[fetchart.Candidate]:
+    def get(self, album, plugin, paths):
+        # type: (AlbumInfo, plugins.BeetsPlugin, List) -> Iterator[fetchart.Candidate]  # noqa
         """Return the url for the cover from the bandcamp album page.
         This only returns cover art urls for bandcamp albums (by id).
         """
         # TODO: Make this configurable
         if hasattr(album, "art_source") and album.art_source == DATA_SOURCE:
             url = album.mb_albumid
             if isinstance(url, six.string_types) and DATA_SOURCE in url:
@@ -107,171 +105,189 @@
                     self._info("Could not connect to the URL")
             else:
                 self._info("Not fetching art for a non-bandcamp album")
         else:
             self._info("Art cover is already present")
 
 
-class BandcampPlugin(BandcampRequestsHandler, plugins.BeetsPlugin):
-    _gurucache: Dict[str, Metaguru]
-
-    media: str
+class BandcampAdditionalData:
+    write: bool
     excluded_extra_fields: Set[str]
+    guru: Callable
+    _info: Callable
+
+    def verify_and_add(
+        self, item: library.Item, get_data: Callable[[str], str], excluded: Set[str]
+    ) -> None:
+        name = "Additional data"
+        for bandcamp_field in set(ADDITIONAL_DATA_MAP).difference(excluded):
+            item_field = ADDITIONAL_DATA_MAP[bandcamp_field]
+
+            if not getattr(item, item_field, None) or (
+                item_field == "comments" and item.comments.startswith("Visit http")
+            ):
+                new_value = get_data(bandcamp_field)
+                if new_value:
+                    setattr(item, item_field, new_value)
+                    self._info("{}: obtained {} for {}", name, bandcamp_field, item)
+            else:
+                self._info("{}: {} field: already present on {}", name, item_field, item)
+
+    def add_additional_data(self, item: library.Item) -> None:
+        """If not excluded, fetch and store:
+        * lyrics
+        * release description as comments
+        """
+        self.verify_and_add(
+            item,
+            partial(getattr, self.guru(item.mb_albumid or item.mb_trackid)),
+            self.excluded_extra_fields,
+        )
+
+        if self.write:
+            item.try_write()
+        item.store()
+
+
+class BandcampPlugin(
+    BandcampRequestsHandler, plugins.BeetsPlugin, BandcampAdditionalData
+):
+    _gurucache: Dict[str, Metaguru]
 
     def __init__(self) -> None:
         super().__init__()
         self.config.add(DEFAULT_CONFIG.copy())
-        # ~~~ DEPRECATED
-        if not self.config["lyrics"]:
-            ADDITIONAL_DATA_MAP.pop("lyrics", None)
-        # ~~~
-        self.media = self.config["preferred_media"].as_str()
+
+        self.write = config["import"]["write"].get()
         self.excluded_extra_fields = set(self.config["exclude_extra_fields"].get())
         self.import_stages = [self.imported]
         self.register_listener("pluginload", self.loaded)
         self._gurucache = dict()
 
+    def imported(self, _: Any, task: Any) -> None:
+        """Import hook for fetching additional data from bandcamp."""
+        for item in task.imported_items():
+            if self._from_bandcamp(item):
+                self.add_additional_data(item)
+
     @staticmethod
-    def _from_bandcamp(clue: Union[Item, str]) -> bool:
+    def _from_bandcamp(clue: Union[library.Item, str]) -> bool:
         """Accepts either an item or the mb_artistid."""
-        if isinstance(clue, Item):
+        if isinstance(clue, library.Item):
             clue = clue.mb_albumid or clue.mb_trackid
-        return "bandcamp" in clue or (
+        return ".bandcamp." in clue or (
             clue.startswith("http") and ("album" in clue or "track" in clue)
         )
 
     def guru(self, url: str, html: Optional[str] = None) -> Optional[Metaguru]:
         """Return cached guru. If there isn't one, fetch the url if html isn't
         already given, initialise guru and add it to the cache. This way they
         can be re-used by separate import stages.
         """
         if url in self._gurucache:
             return self._gurucache[url]
         if not html:
             html = self._get(url)
         if html:
-            self._gurucache[url] = Metaguru(html, self.media)
+            self._gurucache[url] = Metaguru(
+                html,
+                self.config["preferred_media"].as_str(),
+                self.config["include_digital_only_tracks"],
+            )
         return self._gurucache.get(url)
 
-    def add_additional_data(self, item: Item, write: bool = False) -> None:
-        """Fetch and store:
-        * lyrics, if enabled
-        * release description as comments
-        """
-        guru = self.guru(item.mb_albumid or item.mb_trackid)
-
-        backup = ""
-        if item.comments.startswith == "Visit http":
-            backup = item.comments
-            item.comments = ""
-
-        for bandcamp_field, item_field in ADDITIONAL_DATA_MAP.items():
-            if item_field in self.excluded_extra_fields:
-                continue
-
-            if getattr(item, item_field, None):
-                self._info("{} field: already present on {}", item_field, item)
-                continue
-
-            setattr(item, item_field, getattr(guru, bandcamp_field))
-            if getattr(item, item_field, None):
-                self._info("Obtained {} for {}", bandcamp_field, item)
-        if not item.comments:
-            item.comments = backup
-
-        if write:
-            item.try_write()
-        item.store()
-
-    def imported(self, _: Any, task: Any) -> None:
-        """Import hook for fetching additional data from bandcamp."""
-        for item in task.imported_items():
-            if self._from_bandcamp(item):
-                self.add_additional_data(item, write=True)
-
     def loaded(self) -> None:
         """Add our own artsource to the fetchart plugin."""
         # TODO: This is ugly, but i didn't find another way to extend fetchart
         # without declaring a new plugin.
         if self.config["art"]:
             for plugin in plugins.find_plugins():
                 if isinstance(plugin, fetchart.FetchArtPlugin):
                     plugin.sources = [
                         BandcampAlbumArt(plugin._log, self.config)
                     ] + plugin.sources
                     fetchart.ART_SOURCES[DATA_SOURCE] = BandcampAlbumArt
                     fetchart.SOURCE_NAMES[BandcampAlbumArt] = DATA_SOURCE
                     break
 
-    def _cheat_mode(self, item: Item, name: str, _type: str) -> Optional[str]:
+    def _cheat_mode(self, item: library.Item, name: str, _type: str) -> str:
         reimport_url: str = getattr(item, f"mb_{_type}id", "")
         if "bandcamp" in reimport_url:
             return reimport_url
 
         if "Visit" in item.comments:
             match = re.search(r"https:[/a-z.-]+com", item.comments)
             if match:
-                url: str = "{}/{}/{}".format(match.group(), _type, urlify(name))
+                url = "{}/{}/{}".format(match.group(), _type, urlify(name))
                 self._info("Trying our guess {} before searching", url)
                 return url
-        return None
+        return ""
 
     def candidates(self, items, artist, album, va_likely, extra_tags=None):
-        # type: (List[Item], str, str, bool, Optional[JSONDict]) -> Iterator[AlbumInfo]
+        # type: (List[library.Item], str, str, bool, Optional[JSONDict]) -> Iterator[AlbumInfo]  # noqa
         """Return a sequence of AlbumInfo objects that match the
         album whose items are provided.
         """
         if items:
             initial_url = self._cheat_mode(items[0], album, ALBUM_SEARCH)
             initial_guess = self.get_album_info(initial_url) if initial_url else None
             if initial_guess:
                 return iter([initial_guess])
+
         return filter(truth, map(self.get_album_info, self._search(album, ALBUM_SEARCH)))
 
     def item_candidates(self, item, artist, title):
-        # type: (Item, str, str) -> Iterator[TrackInfo]
+        # type: (library.Item, str, str) -> Iterator[TrackInfo]
         """Return a sequence of TrackInfo objects that match the provided item.
         If the track was downloaded directly from bandcamp, it should contain
         a comment saying 'Visit <label-url>' - we look at this first by converting
         title into the format that Bandcamp use.
         """
         initial_url = self._cheat_mode(item, title, TRACK_SEARCH)
         initial_guess = self.get_track_info(initial_url) if initial_url else None
         if initial_guess:
             return iter([initial_guess])
+
         query = title or item.album or artist
         return filter(truth, map(self.get_track_info, self._search(query, TRACK_SEARCH)))
 
     def album_for_id(self, album_id: str) -> Optional[AlbumInfo]:
         """Fetch an album by its bandcamp ID."""
-        return self.get_album_info(album_id)
+        if self._from_bandcamp(album_id):
+            return self.get_album_info(album_id)
+
+        self._info("Not a bandcamp URL, skipping")
+        return None
 
     def track_for_id(self, track_id: str) -> Optional[TrackInfo]:
         """Fetch a track by its bandcamp ID."""
-        return self.get_track_info(track_id)
+        if self._from_bandcamp(track_id):
+            return self.get_track_info(track_id)
+
+        self._info("Not a bandcamp URL, skipping")
+        return None
+
+    def handle(self, guru: Metaguru, attr: str, _id: str) -> Any:
+        try:
+            return getattr(guru, attr)
+        except (KeyError, ValueError, AttributeError):
+            self._info("Failed obtaining {}", _id)
+            return None
 
     def get_album_info(self, url: str) -> Optional[AlbumInfo]:
         """Return an AlbumInfo object for a bandcamp album page.
         If track url is given by mistake, find and fetch the album url instead.
         """
-        include_all = self.config["include_digital_only_tracks"]
         guru = self.guru(url, html=self._get(url))
-        return self.handle(partial(guru.album, include_all), url) if guru else None
+        return self.handle(guru, "album", url) if guru else None
 
     def get_track_info(self, url: str) -> Optional[TrackInfo]:
         """Returns a TrackInfo object for a bandcamp track page."""
         guru = self.guru(url)
-        return self.handle(partial(attrgetter("singleton"), guru), url) if guru else None
-
-    def handle(self, call: Callable, _id: str) -> Any:
-        try:
-            return call()
-        except (KeyError, ValueError, AttributeError):
-            self._info("Failed obtaining {}", _id)
-            return None
+        return self.handle(guru, "singleton", url) if guru else None
 
     def _search(self, query: str, search_type: str = ALBUM_SEARCH) -> Iterator[str]:
         """Return an iterator for item URLs of type search_type matching the query."""
         max_urls = self.config["search_max"].as_number()
         urls: Set[str] = set()
 
         page = 1
@@ -281,18 +297,16 @@
         def next_page_exists() -> bool:
             return bool(re.search(rf"page={page}", html))
 
         self._info("Searching {}s for {}", search_type, query)
         while next_page_exists():
             self._info("Page {}", str(page))
             html = self._get(SEARCH_URL.format(query, page))
-            if not html:
-                break
 
-            for match in re.finditer(pattern, html):
+            for match in re.finditer(pattern, html or ""):
                 if len(urls) == max_urls:
                     break
                 url = match.groups()[0]
                 if url not in urls:
                     urls.add(url)
                     yield url
             else:
```

### Comparing `beetcamp-0.9.1/beetsplug/bandcamp/_metaguru.py` & `beetcamp-0.9.3/beetsplug/bandcamp/_metaguru.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module for parsing bandcamp metadata."""
 import json
 import re
 from datetime import date, datetime
 from functools import reduce
 from math import floor
 from operator import truth
-from string import ascii_lowercase, digits
 from typing import Any, Dict, List, Optional, Pattern, Set, Tuple
 from unicodedata import normalize
 
 from beets.autotag.hooks import AlbumInfo, TrackInfo
 from cached_property import cached_property
 from pkg_resources import get_distribution, parse_version
 from pycountry import countries, subdivisions
@@ -21,62 +20,52 @@
 OFFICIAL = "Official"
 PROMO = "Promotional"
 COUNTRY_OVERRIDES = {
     "Russia": "RU",  # pycountry: Russian Federation
     "The Netherlands": "NL",  # pycountry: Netherlands
     "UK": "GB",  # pycountry: Great Britain
 }
-DATE_FORMAT = "%d %B %Y"
 DATA_SOURCE = "bandcamp"
 WORLDWIDE = "XW"
 DEFAULT_MEDIA = "Digital Media"
 MEDIA_MAP = {
     "VinylFormat": "Vinyl",
     "CDFormat": "CD",
     "CassetteFormat": "Cassette",
     "DigitalFormat": DEFAULT_MEDIA,
 }
-VALID_URL_CHARS = {*ascii_lowercase, *digits}
 
 _catalognum = r"([A-Z][^-.\s\d]+[-.\s]?\d{2,4}(?:[.-]?\d|CD)?)"
-_exclusive = r"[\[( -]*(bandcamp )?(digi(tal)? )?(bonus|only|exclusive)[\])]?"
+_exclusive = r"[*\[( -]*(bandcamp )?(digi(tal)? )?(bonus|only|exclusive)[*\])]?"
 _catalognum_header = r"(?:Catalogue(?: (?:Number|N[or]))?|Cat N[or])\.?:"
 PATTERNS: Dict[str, Pattern] = {
-    "meta": re.compile(r".*datePublished.*", flags=re.MULTILINE),
+    "meta": re.compile(r".*dateModified.*", flags=re.MULTILINE),
     "desc_catalognum": re.compile(rf"{_catalognum_header} ?({_catalognum})"),
     "quick_catalognum": re.compile(rf"\[{_catalognum}\]"),
     "catalognum": re.compile(rf"^{_catalognum}|{_catalognum}$"),
     "catalognum_excl": re.compile(r"(?i:vol(ume)?|artists)|202[01]|(^|\s)C\d\d|\d+/\d+"),
     "digital": re.compile(rf"^DIGI (\d+\.\s?)?|(?i:{_exclusive})"),
     "lyrics": re.compile(r'"lyrics":({[^}]*})'),
-    "release_date": re.compile(r"release[ds] ([\d]{2} [A-Z][a-z]+ [\d]{4})"),
     "track_name": re.compile(
         r"""
 ((?P<track_alt>(^[ABCDEFGH]{1,3}[0-6]|^\d)\d?)\s?[.-]+(?=[^\d]))?
 (\s?(?P<artist>[^-]*)(\s-\s))?
 (?P<title>(\b([^\s]-|-[^\s]|[^-])+$))""",
         re.VERBOSE,
     ),
     "vinyl_name": re.compile(
         r'(?P<count>[1-5]|[Ss]ingle|[Dd]ouble|[Tt]riple)(LP)? ?x? ?((7|10|12)" )?Vinyl'
     ),
 }
 
 
 def urlify(pretty_string: str) -> str:
-    """Make a string bandcamp-url-compatible."""
-    return reduce(
-        lambda p, n: p + n
-        if n in VALID_URL_CHARS
-        else p + "-"
-        if not p.endswith("-")
-        else p,
-        pretty_string.lower().replace("'", ""),
-        "",
-    ).strip("-")
+    """Transform a string into bandcamp url."""
+    name = pretty_string.lower().replace("'", "")
+    return re.sub("--+", "-", re.sub(r"\W", "-", name, flags=re.ASCII)).strip("-")
 
 
 class Helpers:
     @staticmethod
     def get_vinyl_count(name: str) -> int:
         conv = {"single": 1, "double": 2, "triple": 3}
         match = re.search(PATTERNS["vinyl_name"], name)
@@ -90,21 +79,21 @@
         """Return cleaned title and whether this track is digital-only."""
         clean_name = re.sub(PATTERNS["digital"], "", name)
         if clean_name != name:
             return clean_name, True
         return clean_name, False
 
     @staticmethod
-    def parse_track_name(name: str) -> Dict[str, str]:
+    def parse_track_name(name: str) -> Dict[str, Optional[str]]:
         name = re.sub(r" \(free[^)]*\)", "", name, flags=re.IGNORECASE)
         track = {"track_alt": None, "artist": None, "title": name}
         match = re.search(PATTERNS["track_name"], name)
         if match:
             track = match.groupdict()
-        track["main_title"] = re.sub(r"\s?([[(]|f(ea)?t\.).*", "", track["title"])
+        track["main_title"] = re.sub(r"\s?([\[(]|f(ea)?t\.).*", "", str(track["title"]))
         return track
 
     @staticmethod
     def parse_catalognum(album: str, disctitle: str, description: str) -> str:
         for pattern, source in [
             (PATTERNS["desc_catalognum"], description),
             (PATTERNS["quick_catalognum"], album),
@@ -116,19 +105,14 @@
                 try:
                     return next(group for group in match.groups() if group)
                 except StopIteration:
                     continue
         return ""
 
     @staticmethod
-    def parse_release_date(string: str) -> str:
-        match = re.search(PATTERNS["release_date"], string)
-        return match.groups()[0] if match else ""
-
-    @staticmethod
     def get_duration(source: JSONDict) -> int:
         for item in source.get("additionalProperty", []):
             if item.get("name") == "duration_secs":
                 return floor(item.get("value", 0))
         return 0
 
     @staticmethod
@@ -158,81 +142,93 @@
                 _trails.format(excl),
             ]
         )
         pat = re.compile(pattern, flags=re.IGNORECASE)
         return re.sub(pat, "", name).strip() or (args[0] if args else name)
 
     @staticmethod
-    def _get_media(meta: JSONDict) -> JSONDict:
+    def _get_media_index(meta: JSONDict) -> JSONDict:
         """Get release media from the metadata, excluding bundles.
         Return a dictionary with a human mapping (Digital|CD|Vinyl|Cassette) -> media.
         """
         media: JSONDict = {}
         for _format in meta["albumRelease"]:
             try:
-                assert "bundle" not in _format["name"].lower()
+                if "bundle" in _format["name"].lower():
+                    raise KeyError
+
                 medium = _format["musicReleaseFormat"]
-            except (KeyError, AssertionError):
+            except KeyError:
                 continue
             human_name = MEDIA_MAP[medium]
             media[human_name] = _format
         return media
 
 
 class Metaguru(Helpers):
     html: str
-    preferred_media: str
     meta: JSONDict
+    include_all_tracks: bool
 
     _media: Dict[str, str]
-    _all_media = {DEFAULT_MEDIA}  # type: Set[str]
-    _singleton = False  # type: bool
-    _release_datestr = ""
+    _singleton = False
 
-    def __init__(self, html: str, media: str = DEFAULT_MEDIA) -> None:
-        self._media = {}
+    def __init__(
+        self, html: str, media_prefs: str = DEFAULT_MEDIA, include_all_tracks: bool = True
+    ) -> None:
         self.html = html
-        self.preferred_media = media
-
         self.meta = {}
+        self.include_all_tracks = include_all_tracks
+
         match = re.search(PATTERNS["meta"], html)
         if match:
             self.meta = json.loads(match.group())
 
-        match = re.search(PATTERNS["release_date"], html)
-        if match:
-            self._release_datestr = match.groups()[0]
+        self._media = self.meta.get("albumRelease", [{}])[0]
+        try:
+            media_index = self._get_media_index(self.meta)
+        except (KeyError, AttributeError):
+            pass
+        else:
+            # if preference is given and the format is available, use it
+            for preference in media_prefs.split(","):
+                if preference in media_index:
+                    self._media = media_index[preference]
+                    break
 
     @cached_property
     def description(self) -> str:
-        """Return album and media description if unless they start with a generic message.
+        """Return album and media description unless they start with a generic message.
         If credits exist, append them too.
         """
-        exclude = r"Includes high-quality dow.*"
         _credits = self.meta.get("creditText", "")
-        contents = [
+        parts = [
             self.meta.get("description", ""),
-            re.sub(exclude, "", self._media.get("description", "")),
+            "" if self.media_name == DEFAULT_MEDIA else self._media.get("description"),
             "Credits: " + _credits if _credits else "",
         ]
-        s = "\n - "
-        return reduce(lambda a, b: a + s + b if b else a, contents, "").replace("\r", "")
+        return reduce(lambda x, y: x + "\n - " + y, filter(truth, parts), "")
 
     @cached_property
     def album_name(self) -> str:
         match = re.search(r"Title:([^\n]+)", self.description)
         if match:
             return match.groups()[0].strip()
         return self.meta["name"]
 
     @cached_property
     def label(self) -> str:
         match = re.search(r"Label:([^/,\n]+)", self.description)
         if match:
             return match.groups()[0].strip()
+
+        try:
+            return self.meta["albumRelease"][0]["recordLabel"]["name"]
+        except (KeyError, IndexError):
+            pass
         return self.meta["publisher"]["name"]
 
     @cached_property
     def album_id(self) -> str:
         return self.meta["@id"]
 
     @cached_property
@@ -261,29 +257,33 @@
         matches = re.findall(PATTERNS["lyrics"], self.html)
         if not matches:
             return None
         return "\n".join(json.loads(m).get("text") for m in matches)
 
     @cached_property
     def release_date(self) -> date:
-        return datetime.strptime(self._release_datestr, DATE_FORMAT).date()
+        """Parse the datestring that takes the format like below and return date object.
+        {"datePublished": "17 Jul 2020 00:00:00 GMT"}
+        """
+        date_part = re.sub(r"\s[0-9]{2}:.+", "", self.meta["datePublished"])
+        return datetime.strptime(date_part, "%d %b %Y").date()
 
     @cached_property
-    def media(self) -> str:
+    def media_name(self) -> str:
         """Return the human-readable version of the media format."""
         return MEDIA_MAP.get(self._media.get("musicReleaseFormat", ""), DEFAULT_MEDIA)
 
     @cached_property
     def disctitle(self) -> str:
         """Return medium's disc title if found."""
-        return "" if self.media == DEFAULT_MEDIA else self._media.get("name", "")
+        return "" if self.media_name == DEFAULT_MEDIA else self._media.get("name", "")
 
-    @property
+    @cached_property
     def mediums(self) -> int:
-        return self.get_vinyl_count(self.disctitle) if self.media == "Vinyl" else 1
+        return self.get_vinyl_count(self.disctitle) if self.media_name == "Vinyl" else 1
 
     @cached_property
     def catalognum(self) -> str:
         return self.parse_catalognum(self.album_name, self.disctitle, self.description)
 
     @cached_property
     def country(self) -> str:
@@ -291,15 +291,15 @@
             loc = self.meta["publisher"]["foundingLocation"]["name"].rpartition(", ")[-1]
             name = normalize("NFKD", loc).encode("ascii", "ignore").decode()
             return (
                 COUNTRY_OVERRIDES.get(name)
                 or getattr(countries.get(name=name, default=object), "alpha_2", None)
                 or subdivisions.lookup(name).country_code
             )
-        except (KeyError, ValueError, LookupError):
+        except (ValueError, LookupError):
             return WORLDWIDE
 
     @cached_property
     def tracks(self) -> List[JSONDict]:
         """Parse relevant details from the tracks' JSON."""
         if self._singleton:
             raw_tracks = [{"item": self.meta}]
@@ -359,38 +359,38 @@
             return "Various Artists"
         if self.label == self.bandcamp_albumartist:
             artists = self.track_artists
             if len(artists) == 1:
                 return next(iter(artists))
         return self.bandcamp_albumartist
 
-    @property
+    @cached_property
     def albumtype(self) -> str:
         if self.is_lp:
             return "album"
         if self.is_ep:
             return "ep"
         if self.is_single:
             return "single"
         if self.is_va:
             return "compilation"
         return "album"
 
-    @property
+    @cached_property
     def clean_album_name(self) -> str:
-        args = set(filter(truth, [self.catalognum, self.label]))
+        args = list(filter(truth, [self.catalognum, self.label]))
         if not self._singleton:
-            args.add(self.bandcamp_albumartist)
+            args.append(self.bandcamp_albumartist)
         return self.clean_up_album_name(self.album_name, *args)
 
     @property
     def _common(self) -> JSONDict:
         return dict(
             data_source=DATA_SOURCE,
-            media=self.media,
+            media=self.media_name,
             data_url=self.album_id,
             artist_id=self.artist_id,
         )
 
     @property
     def _common_album(self) -> JSONDict:
         return dict(
@@ -401,64 +401,53 @@
             catalognum=self.catalognum,
             albumtype=self.albumtype,
             album=self.clean_album_name,
             albumstatus=OFFICIAL if self.release_date <= date.today() else PROMO,
             country=self.country,
         )
 
-    def _trackinfo(self, track: JSONDict, medium_total: int, **kwargs: Any) -> TrackInfo:
+    def _trackinfo(self, track: JSONDict, **kwargs: Any) -> TrackInfo:
         track.pop("digital_only")
         track.pop("main_title")
         return TrackInfo(
             **self._common,
             **track,
             disctitle=self.disctitle or None,
             medium=1,
-            medium_total=medium_total,
             **kwargs,
         )
 
     @property
     def singleton(self) -> TrackInfo:
         self._singleton = True
-        track = self.tracks[0]
-        track.update(self.parse_track_name(self.album_name))
         kwargs: JSONDict = {}
         if NEW_BEETS:
             kwargs.update(**self._common_album, albumartist=self.bandcamp_albumartist)
 
-        return self._trackinfo(track.copy(), 1, **kwargs)
+        track = self.tracks[0].copy()
+        track.update(self.parse_track_name(self.album_name))
+        if not track.get("artist"):
+            track["artist"] = self.bandcamp_albumartist
+        if NEW_BEETS and "-" not in kwargs.get("album", ""):
+            kwargs["album"] = "{} - {}".format(track["artist"], track["title"])
+
+        return self._trackinfo(track, medium_total=1, **kwargs)
 
-    def albuminfo(self, include_all: bool) -> AlbumInfo:
-        if self.media == "Digital Media" or include_all:
+    @property
+    def album(self) -> AlbumInfo:
+        """Return album for the appropriate release format."""
+        if self.media_name == DEFAULT_MEDIA or self.include_all_tracks:
             filtered_tracks = self.tracks
         else:
             filtered_tracks = [t for t in self.tracks if not t["digital_only"]]
 
-        medium_total = len(filtered_tracks)
-        _tracks = [self._trackinfo(t.copy(), medium_total) for t in filtered_tracks]
+        total = len(filtered_tracks)
+        _tracks = [self._trackinfo(t.copy(), medium_total=total) for t in filtered_tracks]
         return AlbumInfo(
             **self._common,
             **self._common_album,
             artist=self.albumartist,
             album_id=self.album_id,
             va=self.is_va,
             mediums=self.mediums,
             tracks=_tracks,
         )
-
-    def album(self, include_all: bool) -> AlbumInfo:
-        """Return album for the appropriate release format."""
-        try:
-            media = self._get_media(self.meta)
-        except (KeyError, AttributeError):
-            return None
-        self._all_media = set(media)
-        # if preference is given and the format is available, return it
-        for preference in self.preferred_media.split(","):
-            if preference in media:
-                self._media = media[preference]
-                break
-        else:  # otherwise, use the default option
-            self._media = media[DEFAULT_MEDIA]
-
-        return self.albuminfo(include_all)
```

### Comparing `beetcamp-0.9.1/pyproject.toml` & `beetcamp-0.9.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "beetcamp"
-version = "0.9.1"
+version = "0.9.3"
 description = "Bandcamp autotagger source for beets (http://beets.io)."
 authors = ["Šarūnas Nejus <snejus@pm.me>"]
 readme = "README.md"
 license = "GPL-2.0"
-homepage = "https://github.com/snejus/beets-bandcamp"
-repository = "https://github.com/snejus/beets-bandcamp"
+homepage = "https://github.com/snejus/beetcamp"
+repository = "https://github.com/snejus/beetcamp"
 
 packages = [{ include = "beetsplug" }]
 include = ["LICENSE", "README.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.6,<3.10"
 
@@ -19,16 +19,21 @@
 pycountry = "^20.7.3"
 
 [tool.poetry.dev-dependencies]
 beets = { git = "https://github.com/beetbox/beets" }
 dataclasses = { version = "*", python = "<3.7" }
 tox = ">=3.21.1"
 flake8 = ">=3.8.4"
+flake8-bandit = ">=2.0.0"
 mypy = ">=0.790"
 pylint = ">=2.7.4"
 pytest = ">=6.2"
 pytest-cov = ">=2.10.1"
+pytest-randomly = "*"
 pytest-lazy-fixture = ">=0.6.3"
+types-setuptools = "^57.0.0"
+types-requests = "^2.25.0"
+types-six = "^0.1.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beetcamp-0.9.1/setup.py` & `beetcamp-0.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['cached-property>=1.5.2,<2.0.0', 'pycountry>=20.7.3,<21.0.0', 'requests']
 
 setup_kwargs = {
     'name': 'beetcamp',
-    'version': '0.9.1',
+    'version': '0.9.3',
     'description': 'Bandcamp autotagger source for beets (http://beets.io).',
-    'long_description': "[![image](http://img.shields.io/pypi/v/beetcamp.svg)](https://pypi.python.org/pypi/beetcamp)\n\nPlug-in for [beets](https://github.com/beetbox/beets) to use Bandcamp as\nan autotagger source.\n\nThis is an up-to-date fork of [unrblt/beets-bandcamp](https://github.com/unrblt/beets-bandcamp)\n\n# Installation\n\n## Recommended method\n\n1. Install `beets` with `pipx` so that it's isolated from your system and other projects\n```bash\npipx install beets\n```\n\n2. Inject `beetcamp` and other dependencies that you need\n```bash\npipx inject beets beetcamp [python-mpd2 ...]\n```\nand add `bandcamp` to the `plugins` list to your beets configuration file.\n\n## Otherwise\n\nNavigate to your `beets` virtual environment and install the plug-in with\n\n```bash\n   pip install beetcamp\n```\n\n\n\n# Configuration\n\n## Example\n\n```yaml\nbandcamp:\n    preferred_media: Vinyl,CD,Cassette\n    include_digital_only_tracks: true\n    search_max: 5\n    art: true\n    exclude_extra_fields:\n      - lyrics\n      - comments\n```\n---\n\n#### `preferred_media`\n\n- Type: **string**\n- Default: `Digital`\n\nA comma-separated list of media to prioritise when fetching albums. For example:\n`preferred_media: Vinyl,Cassette` will ignore `CD`, check for a `Vinyl`, and then for a\n`Cassette`, in the end defaulting to `Digital` (always available) if none of the two are\nfound. Any combination of the following is supported: `Vinyl`, `CD`, `Cassette`,\n`Digital`.\n\n---\n\n#### `include_digital_only_tracks`\n\n- Type: **bool**\n- Default: `true`\n\nFor media that isn't `Digital Media`, include all tracks, even if their titles contain\n**digital only** (or alike).\n\nIf you have `False` here, then, for example, a `Vinyl` media of an album will only include\nthe tracks that are supposed to be found in that media.\n\n---\n\n#### `search_max`\n\n- Type: **int**\n- Default: `10`.\n\nMaximum number of items to fetch through search queries. Depending on the specificity of\nqueries and whether a suitable match is found, it could fetch 50+ results which may take a\nminute, so it'd make sense to bound this to some sort of sensible number. Usually, a match\nis found among the first 5 items.\n\n---\n\n#### `art`\n\n- Type: **bool**\n- Default: `false`.\n\nAdd a source to the\n[FetchArt](http://beets.readthedocs.org/en/latest/plugins/fetchart.html) plug-in to\ndownload album art for Bandcamp albums (requires `FetchArt` plug-in enabled).\n\n---\n\n#### `exclude_extra_fields`\n\n- Type: **list**\n- Default: _`empty`_\n\nThe data that is added **after** the core auto tagging process is considered extra:\n(currently) `lyrics` and `comments` (release description) fields (see [the data\ntable](#currently-supported--returned-data) for the complete list). Since there yet isn't\nan easy way to preview them before they get applied, you can ignore them if you find them\nirrelevant or inaccurate.\n\nFor example, if you wanted to ignore all the goodies you can specify\n```yaml\nbandcamp:\n    search_max: 5\n    exclude_extra_fields:\n      - lyrics\n      - comments\n```\n\n---\n\n>#### ~~`lyrics`~~\n>\n>- ~~Default: `false`.~~\n>\n>~~Add lyrics to the tracks if they are available.~~\n- deprecated - see `exclude_extra_fields` above\n\n# Usage\n\nThis plug-in uses the Bandcamp URL as id (for both albums and songs). If no matching\nrelease is found when importing you can select `enter Id` and paste the Bandcamp URL.\n\n## Currently supported / returned data\n\n| field            | is extra | singleton track | album track | album |\n|-----------------:|:--------:|:---------------:|:-----------:|:-----:|\n| `album`          |          | ✔~              |             | ✔     |\n| `album_id`       |          |                 |             | ✔     |\n| `albumartist`    |          | ✔               | ✔           | ✔     |\n| `albumstatus`    |          | ✔~              |             | ✔     |\n| `albumtype`      |          | ✔~              |             | ✔     |\n| `artist`         |          | ✔               | ✔           | ✔     |\n| `artist_id`      |          | ✔               | ✔           |       |\n| `catalognum`     |          | ✔~              |             | ✔     |\n| + `comments`     | ✔        | ✔               | ✔           |       |\n| `country`        |          | ✔~              |             | ✔     |\n| `day`            |          | ✔~              |             | ✔     |\n| `disctitle`      |          | ✔~              | ✔           |       |\n| `image`          |          | ✔               | ✔           | ✔     |\n| `index`          |          | ✔               | ✔           |       |\n| `label`          |          | ✔~              | ✔           | ✔     |\n| `length`         |          | ✔               | ✔           |       |\n| `lyrics`         | ✔        | ✔               | ✔           |       |\n| `media`          |          | ✔~              | ✔           | ✔     |\n| `medium`         |          | ✔~              | ✔           |       |\n| `mediums`        |          |                 |             | ✔     |\n| * `medium_index` |          | ✔~              | ✔           |       |\n| * `medium_total` |          | ✔~              | ✔           |       |\n| `month`          |          | ✔~              |             | ✔     |\n| `title`          |          | ✔               | ✔           |       |\n| `track_alt`      |          | ✔               | ✔           |       |\n| `va`             |          |                 |             | ✔     |\n| `year`           |          | ✔~              |             | ✔     |\n\n**\\+** `comments` field gets populated with the release description.\n\n**\\*** are likely to be inaccurate, since Bandcamp does not provide this data,\n  therefore they depend on artists providing some clues in the descriptions of\n  their releases. This is only relevant if you have `per_disc_numbering` set to\n  `True` in the global beets configuration.\n\n**\\~** These singleton fields are available if you use `beets` version `1.5` or higher.\n",
+    'long_description': "[![image](http://img.shields.io/pypi/v/beetcamp.svg)](https://pypi.python.org/pypi/beetcamp)\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=snejus_beets-bandcamp&metric=alert_status)](https://sonarcloud.io/dashboard?id=snejus_beets-bandcamp)\n\nPlug-in for [beets](https://github.com/beetbox/beets) to use Bandcamp as\nan autotagger source.\n\nThis is an up-to-date fork of [unrblt/beets-bandcamp](https://github.com/unrblt/beets-bandcamp)\n\n# Installation\n\n## Recommended method\n\n1. Install `beets` with `pipx` so that it's isolated from your system and other projects\n```bash\npipx install beets\n```\n\n2. Inject `beetcamp` and other dependencies that you need\n```bash\npipx inject beets beetcamp [python-mpd2 ...]\n```\nand add `bandcamp` to the `plugins` list to your beets configuration file.\n\n## Otherwise\n\nNavigate to your `beets` virtual environment and install the plug-in with\n\n```bash\n   pip install beetcamp\n```\n\n\n\n# Configuration\n\n## Example\n\n```yaml\nbandcamp:\n    preferred_media: Vinyl,CD,Cassette\n    include_digital_only_tracks: true\n    search_max: 5\n    art: true\n    exclude_extra_fields:\n      - lyrics\n      - comments\n```\n---\n\n#### `preferred_media`\n\n- Type: **string**\n- Default: `Digital`\n\nA comma-separated list of media to prioritise when fetching albums. For example:\n`preferred_media: Vinyl,Cassette` will ignore `CD`, check for a `Vinyl`, and then for a\n`Cassette`, in the end defaulting to `Digital` (always available) if none of the two are\nfound. Any combination of the following is supported: `Vinyl`, `CD`, `Cassette`,\n`Digital`.\n\n---\n\n#### `include_digital_only_tracks`\n\n- Type: **bool**\n- Default: `true`\n\nFor media that isn't `Digital Media`, include all tracks, even if their titles contain\n**digital only** (or alike).\n\nIf you have `False` here, then, for example, a `Vinyl` media of an album will only include\nthe tracks that are supposed to be found in that media.\n\n---\n\n#### `search_max`\n\n- Type: **int**\n- Default: `10`.\n\nMaximum number of items to fetch through search queries. Depending on the specificity of\nqueries and whether a suitable match is found, it could fetch 50+ results which may take a\nminute, so it'd make sense to bound this to some sort of sensible number. Usually, a match\nis found among the first 5 items.\n\n---\n\n#### `art`\n\n- Type: **bool**\n- Default: `false`.\n\nAdd a source to the\n[FetchArt](http://beets.readthedocs.org/en/latest/plugins/fetchart.html) plug-in to\ndownload album art for Bandcamp albums (requires `FetchArt` plug-in enabled).\n\n---\n\n#### `exclude_extra_fields`\n\n- Type: **list**\n- Default: _`empty`_\n\nThe data that is added **after** the core auto tagging process is considered extra:\n(currently) `lyrics` and `comments` (release description) fields (see [the data\ntable](#currently-supported--returned-data) for the complete list). Since there yet isn't\nan easy way to preview them before they get applied, you can ignore them if you find them\nirrelevant or inaccurate.\n\nFor example, if you wanted to ignore all the goodies you can specify\n```yaml\nbandcamp:\n    search_max: 5\n    exclude_extra_fields:\n      - lyrics\n      - comments\n```\n\n---\n\n>#### ~~`lyrics`~~\n>\n>- ~~Default: `false`.~~\n>\n>~~Add lyrics to the tracks if they are available.~~\n- deprecated - see `exclude_extra_fields` above\n\n# Usage\n\nThis plug-in uses the Bandcamp URL as id (for both albums and songs). If no matching\nrelease is found when importing you can select `enter Id` and paste the Bandcamp URL.\n\n## Currently supported / returned data\n\n| field            | is extra | singleton track | album track | album |\n|-----------------:|:--------:|:---------------:|:-----------:|:-----:|\n| `album`          |          | ✔~              |             | ✔     |\n| `album_id`       |          |                 |             | ✔     |\n| `albumartist`    |          | ✔               | ✔           | ✔     |\n| `albumstatus`    |          | ✔~              |             | ✔     |\n| `albumtype`      |          | ✔~              |             | ✔     |\n| `artist`         |          | ✔               | ✔           | ✔     |\n| `artist_id`      |          | ✔               | ✔           |       |\n| `catalognum`     |          | ✔~              |             | ✔     |\n| + `comments`     | ✔        | ✔               | ✔           |       |\n| `country`        |          | ✔~              |             | ✔     |\n| `day`            |          | ✔~              |             | ✔     |\n| `disctitle`      |          | ✔~              | ✔           |       |\n| `image`          |          | ✔               | ✔           | ✔     |\n| `index`          |          | ✔               | ✔           |       |\n| `label`          |          | ✔~              | ✔           | ✔     |\n| `length`         |          | ✔               | ✔           |       |\n| `lyrics`         | ✔        | ✔               | ✔           |       |\n| `media`          |          | ✔~              | ✔           | ✔     |\n| `medium`         |          | ✔~              | ✔           |       |\n| `mediums`        |          |                 |             | ✔     |\n| * `medium_index` |          | ✔~              | ✔           |       |\n| * `medium_total` |          | ✔~              | ✔           |       |\n| `month`          |          | ✔~              |             | ✔     |\n| `title`          |          | ✔               | ✔           |       |\n| `track_alt`      |          | ✔               | ✔           |       |\n| `va`             |          |                 |             | ✔     |\n| `year`           |          | ✔~              |             | ✔     |\n\n**\\+** `comments` field gets populated with the release description.\n\n**\\*** are likely to be inaccurate, since Bandcamp does not provide this data,\n  therefore they depend on artists providing some clues in the descriptions of\n  their releases. This is only relevant if you have `per_disc_numbering` set to\n  `True` in the global beets configuration.\n\n**\\~** These singleton fields are available if you use `beets` version `1.5` or higher.\n",
     'author': 'Šarūnas Nejus',
     'author_email': 'snejus@pm.me',
     'maintainer': None,
     'maintainer_email': None,
-    'url': 'https://github.com/snejus/beets-bandcamp',
+    'url': 'https://github.com/snejus/beetcamp',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<3.10',
 }
```

### Comparing `beetcamp-0.9.1/PKG-INFO` & `beetcamp-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: beetcamp
-Version: 0.9.1
+Version: 0.9.3
 Summary: Bandcamp autotagger source for beets (http://beets.io).
-Home-page: https://github.com/snejus/beets-bandcamp
+Home-page: https://github.com/snejus/beetcamp
 License: GPL-2.0
 Author: Šarūnas Nejus
 Author-email: snejus@pm.me
 Requires-Python: >=3.6,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: pycountry (>=20.7.3,<21.0.0)
 Requires-Dist: requests
-Project-URL: Repository, https://github.com/snejus/beets-bandcamp
+Project-URL: Repository, https://github.com/snejus/beetcamp
 Description-Content-Type: text/markdown
 
 [![image](http://img.shields.io/pypi/v/beetcamp.svg)](https://pypi.python.org/pypi/beetcamp)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=snejus_beets-bandcamp&metric=alert_status)](https://sonarcloud.io/dashboard?id=snejus_beets-bandcamp)
 
 Plug-in for [beets](https://github.com/beetbox/beets) to use Bandcamp as
 an autotagger source.
 
 This is an up-to-date fork of [unrblt/beets-bandcamp](https://github.com/unrblt/beets-bandcamp)
 
 # Installation
```

