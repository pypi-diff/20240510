# Comparing `tmp/spotify_web_downloader-1.6.6.tar.gz` & `tmp/spotify_web_downloader-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_web_downloader-1.6.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spotify_web_downloader-1.6.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify_web_downloader-1.6.6.tar` & `spotify_web_downloader-1.6.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1137 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/.gitignore
--rw-r--r--   0        0        0     8433 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/README.md
--rw-r--r--   0        0        0      533 2024-04-05 14:54:24.724287 spotify_web_downloader-1.6.6/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/requirements.txt
--rw-r--r--   0        0        0       22 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/__init__.py
--rw-r--r--   0        0        0       30 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/__main__.py
--rw-r--r--   0        0        0    21484 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/cli.py
--rw-r--r--   0        0        0      507 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/constants.py
--rw-r--r--   0        0        0     8546 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/downloader.py
--rw-r--r--   0        0        0    11677 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_music_video.py
--rw-r--r--   0        0        0     9274 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_song.py
--rw-r--r--   0        0        0      177 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/enums.py
--rw-r--r--   0        0        0     4015 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/hardcoded_wvd.py
--rw-r--r--   0        0        0      707 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/models.py
--rw-r--r--   0        0        0     7738 2024-04-05 14:54:24.728287 spotify_web_downloader-1.6.6/spotify_web_downloader/spotify_api.py
--rw-r--r--   0        0        0     8844 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/.gitignore
+-rw-r--r--   0        0        0     9681 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/README.md
+-rw-r--r--   0        0        0      564 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/requirements.txt
+-rw-r--r--   0        0        0       22 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/__main__.py
+-rw-r--r--   0        0        0    23566 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/cli.py
+-rw-r--r--   0        0        0      507 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/constants.py
+-rw-r--r--   0        0        0     9798 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/downloader.py
+-rw-r--r--   0        0        0    13232 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/downloader_music_video.py
+-rw-r--r--   0        0        0    10170 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/downloader_song.py
+-rw-r--r--   0        0        0      246 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/enums.py
+-rw-r--r--   0        0        0     4015 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/hardcoded_wvd.py
+-rw-r--r--   0        0        0      707 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/models.py
+-rw-r--r--   0        0        0     7782 2024-05-10 16:14:52.135727 spotify_web_downloader-1.6.7/spotify_web_downloader/spotify_api.py
+-rw-r--r--   0        0        0    10123 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.7/PKG-INFO
```

### Comparing `spotify_web_downloader-1.6.6/.github/workflows/main.yml` & `spotify_web_downloader-1.6.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.6/README.md` & `spotify_web_downloader-1.6.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 # Spotify Web Downloader
-A Python script to download songs/music videos/albums/playlists directly from Spotify.
+A Python CLI app for downloading songs/music videos/albums/playlists directly from Spotify.
+
+**Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
-* Download songs in 128kbps AAC or in 256kbps AAC with a premium account
+* Download songs in AAC 128kbps or in AAC 256kbps with a premium account
 * Download music videos with a premium account
-* Download synced lyrics
+* Download synced lyrics with a premium account
 * Highly configurable
 
-## Pre-requisites
+## Prerequisites
+* Python 3.8 or higher
 * The cookies file of your Spotify account (free or premium)
-    * You can get your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
+    * You can get your cookies by using one of the following extensions on your browser of choice at the Spotify website with your account signed in:
+        * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
+        * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
 * FFmpeg on your system PATH
     * Older versions of FFmpeg may not work.
-* Python 3.7 or higher
+    * Up to date binaries can be obtained from the links below:
+        * Windows: https://github.com/AnimMouse/ffmpeg-stable-autobuild/releases
+        * Linux: https://johnvansickle.com/ffmpeg/
 
 ## Installation
 1. Install the package `spotify-web-downloader` using pip
     ```bash
     pip install spotify-web-downloader
     ```
-2. Place your cookies in the same directory you will run the script from and name it `cookies.txt`
+2. Place your cookies file in the directory from which you will be running spotify-web-downloader and name it `cookies.txt`.
 
 ## Usage
+```bash
+spotify-web-downloader [OPTIONS] URLS...
+```
+
+### Examples
 * Download a song
     ```bash
     spotify-web-downloader "https://open.spotify.com/track/18gqCQzqYb0zvurQPlRkpo"
     ```
 * Download an album
     ```bash
     spotify-web-downloader "https://open.spotify.com/album/0r8D5N674HbTXlR3zNxeU1"
@@ -45,30 +57,34 @@
 | `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
 | `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
 | `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
 | `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Spotify`                                  |
 | `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
 | `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
 | `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
 | `--aria2c-path` / `aria2c_path`                                 | Path to aria2c binary.                                                       | `aria2c`                                     |
 | `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
 | `--date-tag-template` / `date_tag_template`                     | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
 | `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
 | `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
 | `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                            | `{album_artist}/{album}`                     |
 | `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.                | `Compilations/{album}`                       |
 | `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string.        | `{track:02d} {title}`                        |
 | `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.         | `{disc}-{track:02d} {title}`                 |
 | `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ytdlp`                                      |
 | `--premium-quality`, `-p` / `premium_quality`                   | Download songs in premium quality.                                           | `false`                                      |
 | `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                      | `{artist}/Unknown Album`                     |
 | `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                        | `{title}`                                    |
-| `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ydlp`                                       |
+| `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ytdlp`                                      |
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
+
 ### Tag variables
 The following variables can be used in the template folder/file and/or in the `exclude_tags` list:
 - `album`
 - `album_artist`
 - `artist`
 - `compilation`
 - `composer`
@@ -84,19 +100,26 @@
 - `rating`
 - `release_date`
 - `release_year`
 - `title`
 - `track`
 - `track_total`
 - `url`
+  
+### Remux modes
+The following remux modes are available:
+* `ffmpeg`
+* `mp4box`
+    * Requires mp4decrypt
+    * Can be obtained from here: https://gpac.wp.imt.fr/downloads
 
 ### Music videos quality
 Music videos will be downloaded in the highest quality available in H.264/AAC, up to 1080p.
 
-### Download mode
+### Download modes
 The following modes are available for songs:
 * `ytdlp`
 * `aria2c`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/aria2/aria2/releases
 
 The following modes are available for videos:
```

### Comparing `spotify_web_downloader-1.6.6/pyproject.toml` & `spotify_web_downloader-1.6.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "spotify-web-downloader"
-description = "Download songs/albums/playlists directly from Spotify in AAC"
-requires-python = ">=3.7"
+description = "A Python CLI app for downloading songs/music videos/albums/playlists directly from Spotify."
+requires-python = ">=3.8"
 authors = [{ name = "glomatico" }]
 dependencies = ["click", "pybase62", "pywidevine", "pyyaml", "yt-dlp"]
 readme = "README.md"
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/glomatico/spotify-web-downloader"
```

### Comparing `spotify_web_downloader-1.6.6/spotify_web_downloader/cli.py` & `spotify_web_downloader-1.6.7/spotify_web_downloader/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import click
 
 from . import __version__
 from .constants import *
 from .downloader import Downloader
 from .downloader_music_video import DownloaderMusicVideo
 from .downloader_song import DownloaderSong
-from .enums import DownloadModeSong, DownloadModeVideo
+from .enums import DownloadModeSong, DownloadModeVideo, RemuxMode
 from .models import Lyrics
 from .spotify_api import SpotifyApi
 
 spotify_api_sig = inspect.signature(SpotifyApi.__init__)
 downloader_sig = inspect.signature(Downloader.__init__)
 downloader_song_sig = inspect.signature(DownloaderSong.__init__)
 downloader_music_video_sig = inspect.signature(DownloaderMusicVideo.__init__)
@@ -61,14 +61,15 @@
             ctx.params[param.name] = param.type_cast_value(ctx, config_file[param.name])
     return ctx
 
 
 @click.command()
 @click.help_option("-h", "--help")
 @click.version_option(__version__, "-v", "--version")
+# CLI specific options
 @click.argument(
     "urls",
     nargs=-1,
     type=str,
     required=True,
 )
 @click.option(
@@ -117,21 +118,23 @@
     help="Log level.",
 )
 @click.option(
     "--print-exceptions",
     is_flag=True,
     help="Print exceptions.",
 )
+# API specific options
 @click.option(
     "--cookies-path",
     "-c",
     type=Path,
     default=spotify_api_sig.parameters["cookies_path"].default,
     help="Path to .txt cookies file.",
 )
+# Downloader specific options
 @click.option(
     "--output-path",
     "-o",
     type=Path,
     default=downloader_sig.parameters["output_path"].default,
     help="Path to output directory.",
 )
@@ -150,26 +153,44 @@
 @click.option(
     "--ffmpeg-path",
     type=str,
     default=downloader_sig.parameters["ffmpeg_path"].default,
     help="Path to FFmpeg binary.",
 )
 @click.option(
+    "--mp4box-path",
+    type=str,
+    default=downloader_sig.parameters["mp4box_path"].default,
+    help="Path to MP4Box binary.",
+)
+@click.option(
+    "--mp4decrypt-path",
+    type=str,
+    default=downloader_sig.parameters["mp4decrypt_path"].default,
+    help="Path to mp4decrypt binary.",
+)
+@click.option(
     "--aria2c-path",
     type=str,
     default=downloader_sig.parameters["aria2c_path"].default,
     help="Path to aria2c binary.",
 )
 @click.option(
     "--nm3u8dlre-path",
     type=str,
     default=downloader_sig.parameters["nm3u8dlre_path"].default,
     help="Path to N_m3u8DL-RE binary.",
 )
 @click.option(
+    "--remux-mode",
+    type=RemuxMode,
+    default=downloader_sig.parameters["remux_mode"].default,
+    help="Remux mode.",
+)
+@click.option(
     "--date-tag-template",
     type=str,
     default=downloader_sig.parameters["date_tag_template"].default,
     help="Date tag template.",
 )
 @click.option(
     "--exclude-tags",
@@ -179,14 +200,15 @@
 )
 @click.option(
     "--truncate",
     type=int,
     default=downloader_sig.parameters["truncate"].default,
     help="Maximum length of the file/folder names.",
 )
+# DownloaderSong specific options
 @click.option(
     "--template-folder-album",
     type=str,
     default=downloader_song_sig.parameters["template_folder_album"].default,
     help="Template of the album folders as a format string.",
 )
 @click.option(
@@ -216,14 +238,15 @@
 @click.option(
     "--premium-quality",
     "-p",
     is_flag=True,
     default=downloader_song_sig.parameters["premium_quality"].default,
     help="Download songs in premium quality.",
 )
+# DownloaderMusicVideo specific options
 @click.option(
     "--template-folder-music-video",
     type=str,
     default=downloader_music_video_sig.parameters["template_folder"].default,
     help="Template of the music video folders as a format string.",
 )
 @click.option(
@@ -234,14 +257,15 @@
 )
 @click.option(
     "--download-mode-video",
     type=DownloadModeVideo,
     default=downloader_music_video_sig.parameters["download_mode"].default,
     help="Download mode for videos.",
 )
+# This option should always be last
 @click.option(
     "--no-config-file",
     "-n",
     is_flag=True,
     callback=load_config_file,
     help="Do not use a config file.",
 )
@@ -257,16 +281,19 @@
     log_level: str,
     print_exceptions: bool,
     cookies_path: Path,
     output_path: Path,
     temp_path: Path,
     wvd_path: Path,
     ffmpeg_path: str,
+    mp4box_path: str,
+    mp4decrypt_path: str,
     aria2c_path: str,
     nm3u8dlre_path: str,
+    remux_mode: RemuxMode,
     date_tag_template: str,
     exclude_tags: str,
     truncate: int,
     template_folder_album: str,
     template_folder_compilation: str,
     template_file_single_disc: str,
     template_file_multi_disc: str,
@@ -280,23 +307,29 @@
     logging.basicConfig(
         format="[%(levelname)-8s %(asctime)s] %(message)s",
         datefmt="%H:%M:%S",
     )
     logger = logging.getLogger(__name__)
     logger.setLevel(log_level)
     logger.debug("Starting downloader")
+    if not cookies_path.exists():
+        logger.critical(X_NOT_FOUND_STRING.format("Cookies file", cookies_path))
+        return
     spotify_api = SpotifyApi(cookies_path)
     downloader = Downloader(
         spotify_api,
         output_path,
         temp_path,
         wvd_path,
         ffmpeg_path,
+        mp4box_path,
+        mp4decrypt_path,
         aria2c_path,
         nm3u8dlre_path,
+        remux_mode,
         date_tag_template,
         exclude_tags,
         truncate,
     )
     downloader_song = DownloaderSong(
         downloader,
         template_folder_album,
@@ -308,35 +341,46 @@
     )
     downloader_music_video = DownloaderMusicVideo(
         downloader,
         template_folder_music_video,
         template_file_music_video,
         download_mode_video,
     )
+    if not spotify_api.is_premium:
+        logger.warning("Free account detected, lyrics will not be downloaded")
     if not lrc_only:
         if wvd_path and not wvd_path.exists():
             logger.critical(X_NOT_FOUND_STRING.format(".wvd file", wvd_path))
             return
         logger.debug("Setting up CDM")
         downloader.set_cdm()
-        if not downloader.ffmpeg_path_full:
+        if not downloader.ffmpeg_path_full and remux_mode == RemuxMode.FFMPEG:
             logger.critical(X_NOT_FOUND_STRING.format("ffmpeg", ffmpeg_path))
             return
         if (
             download_mode_song == DownloadModeSong.ARIA2C
             and not downloader.aria2c_path_full
         ):
             logger.critical(X_NOT_FOUND_STRING.format("aria2c", aria2c_path))
             return
         if (
             download_mode_video == DownloadModeVideo.NM3U8DLRE
             and not downloader.nm3u8dlre_path_full
         ):
             logger.critical(X_NOT_FOUND_STRING.format("nm3u8dlre", nm3u8dlre_path))
             return
+        if remux_mode == RemuxMode.MP4BOX:
+            if not downloader.mp4box_path_full:
+                logger.critical(X_NOT_FOUND_STRING.format("MP4Box", mp4box_path))
+                return
+            if not downloader.mp4decrypt_path_full:
+                logger.critical(
+                    X_NOT_FOUND_STRING.format("mp4decrypt", mp4decrypt_path)
+                )
+                return
         if not spotify_api.is_premium and premium_quality:
             logger.critical("Cannot download in premium quality with a free account")
             return
         if not spotify_api.is_premium and download_music_video:
             logger.critical("Cannot download music videos with a free account")
             return
     error_count = 0
@@ -378,15 +422,15 @@
                         spotify_api.track_id_to_gid(music_video_id)
                     )
                     logger.warning(
                         f"({queue_progress}) Switching to download music video "
                         f"with title \"{metadata_gid['name']}\""
                     )
                 if not metadata_gid.get("original_video"):
-                    if metadata_gid.get("has_lyrics"):
+                    if metadata_gid.get("has_lyrics") and spotify_api.is_premium:
                         logger.debug("Getting lyrics")
                         lyrics = downloader_song.get_lyrics(track_id)
                     else:
                         lyrics = Lyrics()
                     logger.debug("Getting album metadata")
                     album_metadata = spotify_api.get_album(
                         spotify_api.gid_to_track_id(metadata_gid["album"]["gid"])
@@ -421,27 +465,29 @@
                         logger.debug("Getting PSSH")
                         pssh = spotify_api.get_pssh(file_id)
                         logger.debug("Getting decryption key")
                         decryption_key = downloader_song.get_decryption_key(pssh)
                         logger.debug("Getting stream URL")
                         stream_url = spotify_api.get_stream_url(file_id)
                         encrypted_path = downloader.get_encrypted_path(track_id, ".m4a")
+                        decrypted_path = downloader.get_decrypted_path(track_id, ".m4a")
                         logger.debug(f'Downloading to "{encrypted_path}"')
                         downloader_song.download(encrypted_path, stream_url)
-                        fixed_path = downloader.get_fixed_path(track_id, ".m4a")
-                        logger.debug(f'Remuxing to "{fixed_path}"')
-                        downloader_song.fixup(
-                            decryption_key,
+                        remuxed_path = downloader.get_remuxed_path(track_id, ".m4a")
+                        logger.debug(f'Decrypting/Remuxing to "{remuxed_path}"')
+                        downloader_song.remux(
                             encrypted_path,
-                            fixed_path,
+                            decrypted_path,
+                            remuxed_path,
+                            decryption_key,
                         )
                         logger.debug("Applying tags")
-                        downloader.apply_tags(fixed_path, tags, cover_url)
+                        downloader.apply_tags(remuxed_path, tags, cover_url)
                         logger.debug(f'Moving to "{final_path}"')
-                        downloader.move_to_final_path(fixed_path, final_path)
+                        downloader.move_to_final_path(remuxed_path, final_path)
                     if no_lrc or not lyrics.synced:
                         pass
                     elif lrc_path.exists() and not overwrite:
                         logger.debug(
                             f'Synced lyrics already exists at "{lrc_path}", skipping'
                         )
                     else:
@@ -507,44 +553,52 @@
                         )
                         m3u8_path_video = downloader_music_video.get_m3u8_path(
                             track_id, "video"
                         )
                         encrypted_path_video = downloader.get_encrypted_path(
                             track_id, "_video.ts"
                         )
+                        decrypted_path_video = downloader.get_decrypted_path(
+                            track_id, "_video.ts"
+                        )
                         logger.debug(f'Downloading video to "{encrypted_path_video}"')
                         downloader_music_video.save_m3u8(m3u8.video, m3u8_path_video)
                         downloader_music_video.download(
                             m3u8_path_video,
                             encrypted_path_video,
                         )
                         m3u8_path_audio = downloader_music_video.get_m3u8_path(
                             track_id, "audio"
                         )
                         encrypted_path_audio = downloader.get_encrypted_path(
                             track_id, "_audio.ts"
                         )
+                        decrypted_path_audio = downloader.get_decrypted_path(
+                            track_id, "_audio.ts"
+                        )
                         logger.debug(f"Downloading audio to {encrypted_path_audio}")
                         downloader_music_video.save_m3u8(m3u8.audio, m3u8_path_audio)
                         downloader_music_video.download(
                             m3u8_path_audio,
                             encrypted_path_audio,
                         )
-                        fixed_path = downloader.get_fixed_path(track_id, ".mp4")
-                        logger.debug(f'Remuxing to "{fixed_path}"')
-                        downloader_music_video.fixup(
+                        remuxed_path = downloader.get_remuxed_path(track_id, ".m4v")
+                        logger.debug(f'Decrypting/Remuxing to "{remuxed_path}"')
+                        downloader_music_video.remux(
                             decryption_key,
                             encrypted_path_video,
                             encrypted_path_audio,
-                            fixed_path,
+                            decrypted_path_video,
+                            decrypted_path_audio,
+                            remuxed_path,
                         )
                         logger.debug("Applying tags")
-                        downloader.apply_tags(fixed_path, tags, cover_url)
+                        downloader.apply_tags(remuxed_path, tags, cover_url)
                         logger.debug(f'Moving to "{final_path}"')
-                        downloader.move_to_final_path(fixed_path, final_path)
+                        downloader.move_to_final_path(remuxed_path, final_path)
                     if save_cover:
                         cover_path = downloader_music_video.get_cover_path(final_path)
                         if cover_path.exists() and not overwrite:
                             logger.debug(
                                 f'Cover already exists at "{cover_path}", skipping'
                             )
                         else:
```

### Comparing `spotify_web_downloader-1.6.6/spotify_web_downloader/downloader.py` & `spotify_web_downloader-1.6.7/spotify_web_downloader/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import datetime
 import functools
 import re
 import shutil
+import subprocess
 from pathlib import Path
 
 import requests
 from mutagen.mp4 import MP4, MP4Cover, MP4FreeForm
 from pywidevine import Cdm, Device
 
 from .constants import *
+from .enums import RemuxMode
 from .hardcoded_wvd import HARDCODED_WVD
 from .models import DownloadQueueItem, UrlInfo
 from .spotify_api import SpotifyApi
 
 
 class Downloader:
     ILLEGAL_CHARACTERS_REGEX = r'[\\/:*?"<>|;]'
@@ -22,51 +24,69 @@
     def __init__(
         self,
         spotify_api: SpotifyApi,
         output_path: Path = Path("./Spotify"),
         temp_path: Path = Path("./temp"),
         wvd_path: Path = None,
         ffmpeg_path: str = "ffmpeg",
+        mp4box_path: str = "MP4Box",
+        mp4decrypt_path: str = "mp4decrypt",
         aria2c_path: str = "aria2c",
         nm3u8dlre_path: str = "N_m3u8DL-RE",
+        remux_mode: RemuxMode = RemuxMode.FFMPEG,
         date_tag_template: str = "%Y-%m-%dT%H:%M:%SZ",
         exclude_tags: str = None,
         truncate: int = 40,
-        no_progress: bool = False,
+        silence: bool = False,
     ):
         self.spotify_api = spotify_api
         self.output_path = output_path
         self.temp_path = temp_path
         self.wvd_path = wvd_path
         self.ffmpeg_path = ffmpeg_path
+        self.mp4box_path = mp4box_path
+        self.mp4decrypt_path = mp4decrypt_path
         self.aria2c_path = aria2c_path
         self.nm3u8dlre_path = nm3u8dlre_path
+        self.remux_mode = remux_mode
         self.date_tag_template = date_tag_template
         self.exclude_tags = exclude_tags
         self.truncate = truncate
-        self.no_progress = no_progress
+        self.silence = silence
         self._set_binaries_full_path()
         self._set_exclude_tags_list()
         self._set_truncate()
+        self._set_subprocess_additional_args()
 
     def _set_binaries_full_path(self):
         self.ffmpeg_path_full = shutil.which(self.ffmpeg_path)
+        self.mp4box_path_full = shutil.which(self.mp4box_path)
+        self.mp4decrypt_path_full = shutil.which(self.mp4decrypt_path)
         self.aria2c_path_full = shutil.which(self.aria2c_path)
         self.nm3u8dlre_path_full = shutil.which(self.nm3u8dlre_path)
 
     def _set_exclude_tags_list(self):
         self.exclude_tags_list = (
             [i.lower() for i in self.exclude_tags.split(",")]
             if self.exclude_tags is not None
             else []
         )
 
     def _set_truncate(self):
         self.truncate = None if self.truncate < 4 else self.truncate
 
+    def _set_subprocess_additional_args(self):
+        if self.silence:
+            self.subprocess_additional_args = {
+                "stdout": subprocess.DEVNULL,
+                "stderr": subprocess.DEVNULL,
+            }
+        else:
+            self.subprocess_additional_args = {}
+
     def set_cdm(self) -> None:
         if self.wvd_path:
             self.cdm = Cdm.from_device(Device.load(self.wvd_path))
         else:
             self.cdm = Cdm.from_device(Device.loads(HARDCODED_WVD))
 
     def get_url_info(self, url: str) -> UrlInfo:
@@ -155,73 +175,94 @@
     def get_encrypted_path(
         self,
         track_id: str,
         file_extension: str,
     ) -> Path:
         return self.temp_path / (f"{track_id}_encrypted" + file_extension)
 
-    def get_fixed_path(
+    def get_decrypted_path(
+        self,
+        track_id: str,
+        file_extension: str,
+    ) -> Path:
+        return self.temp_path / (f"{track_id}_decrypted" + file_extension)
+
+    def get_remuxed_path(
         self,
         track_id: str,
         file_extension: str,
     ) -> Path:
-        return self.temp_path / (f"{track_id}_fixed" + file_extension)
+        return self.temp_path / (f"{track_id}_remuxed" + file_extension)
+
+    def decrypt_mp4decrypt(
+        self,
+        encrypted_path: Path,
+        decrypted_path: Path,
+        decryption_key: str,
+    ):
+        subprocess.run(
+            [
+                self.mp4decrypt_path_full,
+                encrypted_path,
+                "--key",
+                f"1:{decryption_key}",
+                decrypted_path,
+            ],
+            check=True,
+            **self.subprocess_additional_args,
+        )
 
     @staticmethod
     @functools.lru_cache()
     def get_image_bytes(url: str) -> bytes:
         return requests.get(url).content
 
     def apply_tags(self, fixed_location: Path, tags: dict, cover_url: str):
-        mp4_tags = {
-            v: [tags[k]]
-            for k, v in MP4_TAGS_MAP.items()
-            if k not in self.exclude_tags_list and tags.get(k) is not None
-        }
-        if not {"track", "track_total"} & set(self.exclude_tags_list) and tags.get(
-            "track"
-        ):
-            mp4_tags["trkn"] = [[0, 0]]
-        if not {"disc", "disc_total"} & set(self.exclude_tags_list) and tags.get(
-            "disc"
-        ):
-            mp4_tags["disk"] = [[0, 0]]
-        if (
-            "compilation" not in self.exclude_tags_list
-            and tags.get("compilation") is not None
-        ):
-            mp4_tags["cpil"] = tags["compilation"]
+        to_apply_tags = [
+            tag_name
+            for tag_name in tags.keys()
+            if tag_name not in self.exclude_tags_list
+        ]
+        mp4_tags = {}
+        for tag_name in to_apply_tags:
+            if tag_name in ("disc", "disc_total"):
+                if mp4_tags.get("disk") is None:
+                    mp4_tags["disk"] = [[0, 0]]
+                if tag_name == "disc":
+                    mp4_tags["disk"][0][0] = tags[tag_name]
+                elif tag_name == "disc_total":
+                    mp4_tags["disk"][0][1] = tags[tag_name]
+            elif tag_name in ("track", "track_total"):
+                if mp4_tags.get("trkn") is None:
+                    mp4_tags["trkn"] = [[0, 0]]
+                if tag_name == "track":
+                    mp4_tags["trkn"][0][0] = tags[tag_name]
+                elif tag_name == "track_total":
+                    mp4_tags["trkn"][0][1] = tags[tag_name]
+            elif tag_name == "compilation":
+                mp4_tags["cpil"] = tags["compilation"]
+            elif tag_name == "isrc":
+                mp4_tags["----:com.apple.iTunes:ISRC"] = [
+                    MP4FreeForm(tags["isrc"].encode("utf-8"))
+                ]
+            elif tag_name == "label":
+                mp4_tags["----:com.apple.iTunes:LABEL"] = [
+                    MP4FreeForm(tags["label"].encode("utf-8"))
+                ]
+            elif (
+                MP4_TAGS_MAP.get(tag_name) is not None
+                and tags.get(tag_name) is not None
+            ):
+                mp4_tags[MP4_TAGS_MAP[tag_name]] = [tags[tag_name]]
         if "cover" not in self.exclude_tags_list:
             mp4_tags["covr"] = [
                 MP4Cover(
                     self.get_image_bytes(cover_url), imageformat=MP4Cover.FORMAT_JPEG
                 )
             ]
-        if "isrc" not in self.exclude_tags_list and tags.get("isrc") is not None:
-            mp4_tags["----:com.apple.iTunes:ISRC"] = [
-                MP4FreeForm(tags["isrc"].encode("utf-8"))
-            ]
-        if "label" not in self.exclude_tags_list and tags.get("label") is not None:
-            mp4_tags["----:com.apple.iTunes:LABEL"] = [
-                MP4FreeForm(tags["label"].encode("utf-8"))
-            ]
-        if "track" not in self.exclude_tags_list and tags.get("track") is not None:
-            mp4_tags["trkn"][0][0] = tags["track"]
-        if (
-            "track_total" not in self.exclude_tags_list
-            and tags.get("track_total") is not None
-        ):
-            mp4_tags["trkn"][0][1] = tags["track_total"]
-        if "disc" not in self.exclude_tags_list and tags.get("disc") is not None:
-            mp4_tags["disk"][0][0] = tags["disc"]
-        if (
-            "disc_total" not in self.exclude_tags_list
-            and tags.get("disc_total") is not None
-        ):
-            mp4_tags["disk"][0][1] = tags["disc_total"]
         mp4 = MP4(fixed_location)
         mp4.clear()
         mp4.update(mp4_tags)
         mp4.save()
 
     def move_to_final_path(self, fixed_path: Path, final_path: Path):
         final_path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `spotify_web_downloader-1.6.6/spotify_web_downloader/downloader_music_video.py` & `spotify_web_downloader-1.6.7/spotify_web_downloader/downloader_song.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,213 +1,101 @@
-from __future__ import annotations
-
+import datetime
 import subprocess
 from pathlib import Path
 
 from pywidevine import PSSH
 from yt_dlp import YoutubeDL
 
 from .downloader import Downloader
-from .enums import DownloadModeVideo
-from .models import VideoM3U8, VideoStreamInfo
-
+from .enums import DownloadModeSong, RemuxMode
+from .models import Lyrics
 
-class DownloaderMusicVideo:
-    M3U8_HEADER = """#EXTM3U
-#EXT-X-VERSION:3
-#EXT-X-PLAYLIST-TYPE:VOD
-#EXT-X-MEDIA-SEQUENCE:0
-#EXT-X-TARGETDURATION:1"""
 
+class DownloaderSong:
     def __init__(
         self,
         downloader: Downloader,
-        template_folder: str = "{artist}/Unknown Album",
-        template_file: str = "{title}",
-        download_mode: DownloadModeVideo = DownloadModeVideo.YTDLP,
+        template_folder_album: str = "{album_artist}/{album}",
+        template_folder_compilation: str = "Compilations/{album}",
+        template_file_single_disc: str = "{track:02d} {title}",
+        template_file_multi_disc: str = "{disc}-{track:02d} {title}",
+        download_mode: DownloadModeSong = DownloadModeSong.YTDLP,
+        premium_quality: bool = False,
     ):
         self.downloader = downloader
-        self.template_folder = template_folder
-        self.template_file = template_file
+        self.template_folder_album = template_folder_album
+        self.template_folder_compilation = template_folder_compilation
+        self.template_file_single_disc = template_file_single_disc
+        self.template_file_multi_disc = template_file_multi_disc
         self.download_mode = download_mode
+        self.premium_quality = premium_quality
+        self._set_codec()
 
-    def get_music_video_id_from_song_id(
-        self,
-        track_id: str,
-        artist_id: str,
-    ) -> dict | None:
-        now_playing_view = self.downloader.spotify_api.get_now_playing_view(
-            track_id, artist_id
-        )
-        related_music_videos = now_playing_view["data"]["trackUnion"]["relatedVideos"][
-            "items"
-        ]
-        if not related_music_videos:
-            return
-        return related_music_videos[0]["trackOfVideo"]["data"]["uri"].split(":")[-1]
+    def _set_codec(self):
+        self.codec = "MP4_256" if self.premium_quality else "MP4_128"
 
     def get_final_path(self, tags: dict) -> Path:
-        final_path_folder = self.template_folder.split("/")
-        final_path_file = self.template_file.split("/")
+        final_path_folder = (
+            self.template_folder_compilation.split("/")
+            if tags["compilation"]
+            else self.template_folder_album.split("/")
+        )
+        final_path_file = (
+            self.template_file_multi_disc.split("/")
+            if tags["disc_total"] > 1
+            else self.template_file_single_disc.split("/")
+        )
         final_path_folder = [
             self.downloader.get_sanitized_string(i.format(**tags), True)
             for i in final_path_folder
         ]
         final_path_file = [
             self.downloader.get_sanitized_string(i.format(**tags), True)
             for i in final_path_file[:-1]
         ] + [
             self.downloader.get_sanitized_string(
                 final_path_file[-1].format(**tags), False
             )
-            + ".mp4"
+            + ".m4a"
         ]
         return self.downloader.output_path.joinpath(*final_path_folder).joinpath(
             *final_path_file
         )
 
-    def get_manifest(self, metadata_gid: dict) -> dict:
-        return self.downloader.spotify_api.get_video_manifest(
-            metadata_gid["original_video"][0]["gid"]
-        )
-
-    def get_video_stream_info(self, manifest: dict) -> VideoStreamInfo:
-        video_formats = list(
-            format
-            for format in manifest["contents"][0]["profiles"]
-            if format.get("video_bitrate") and format["file_type"] == "mp4"
-        )
-        audio_formats = list(
-            format
-            for format in manifest["contents"][0]["profiles"]
-            if format.get("audio_bitrate") and format["file_type"] == "mp4"
-        )
-        best_video_format = max(video_formats, key=lambda x: x["video_bitrate"])
-        best_audio_format = max(audio_formats, key=lambda x: x["audio_bitrate"])
-        base_url = manifest["base_urls"][0]
-        initialization_template_url = manifest["initialization_template"]
-        segment_template_url = manifest["segment_template"]
-        end_time_millis = manifest["end_time_millis"]
-        segment_length = manifest["contents"][0]["segment_length"]
-        profile_id_video = best_video_format["id"]
-        profile_id_audio = best_audio_format["id"]
-        file_type_video = best_video_format["file_type"]
-        file_type_audio = best_audio_format["file_type"]
-        pssh = next(
-            encryption_info
-            for encryption_info in manifest["contents"][0]["encryption_infos"]
-            if encryption_info["key_system"] == "widevine"
-        )["encryption_data"]
-        return VideoStreamInfo(
-            base_url,
-            initialization_template_url,
-            segment_template_url,
-            end_time_millis,
-            segment_length,
-            profile_id_video,
-            profile_id_audio,
-            file_type_video,
-            file_type_audio,
-            pssh,
-        )
-
     def get_decryption_key(self, pssh: str) -> str:
-        pssh = PSSH(pssh)
-        cdm_session = self.downloader.cdm.open()
-        challenge = self.downloader.cdm.get_license_challenge(cdm_session, pssh)
-        license = self.downloader.spotify_api.get_widevine_license_video(challenge)
-        self.downloader.cdm.parse_license(cdm_session, license)
-        decryption_key = next(
-            i for i in self.downloader.cdm.get_keys(cdm_session) if i.type == "CONTENT"
-        ).key.hex()
-        self.downloader.cdm.close(cdm_session)
+        try:
+            pssh = PSSH(pssh)
+            cdm_session = self.downloader.cdm.open()
+            challenge = self.downloader.cdm.get_license_challenge(cdm_session, pssh)
+            license = self.downloader.spotify_api.get_widevine_license_music(challenge)
+            self.downloader.cdm.parse_license(cdm_session, license)
+            decryption_key = next(
+                i
+                for i in self.downloader.cdm.get_keys(cdm_session)
+                if i.type == "CONTENT"
+            ).key.hex()
+        finally:
+            self.downloader.cdm.close(cdm_session)
         return decryption_key
 
-    def get_m3u8_path(self, track_id: str, type: str) -> Path:
-        return self.downloader.temp_path / f"{track_id}_{type}.m3u8"
-
-    def get_cover_path(self, final_path: Path) -> Path:
-        return final_path.with_suffix(".jpg")
-
-    def get_m3u8_str(self, segments: list) -> str:
-        return (
-            self.M3U8_HEADER
-            + "\n"
-            + "\n".join(f"#EXTINF:1,\n{i}" for i in segments)
-            + "\n"
-            + "#EXT-X-ENDLIST"
-        )
-
-    def get_m3u8(
-        self,
-        base_url: str,
-        initialization_template_url: str,
-        segment_template_url: str,
-        end_time_millis: int,
-        segment_length: int,
-        profile_id_video: int,
-        profile_id_audio: int,
-        file_type_video: str,
-        file_type_audio: str,
-    ) -> VideoM3U8:
-        segments_video, segments_audio = self.get_segment_urls(
-            base_url,
-            initialization_template_url,
-            segment_template_url,
-            end_time_millis,
-            segment_length,
-            profile_id_video,
-            file_type_video,
-        ), self.get_segment_urls(
-            base_url,
-            initialization_template_url,
-            segment_template_url,
-            end_time_millis,
-            segment_length,
-            profile_id_audio,
-            file_type_audio,
-        )
-        m3u8_video = self.get_m3u8_str(segments_video)
-        m3u8_audio = self.get_m3u8_str(segments_audio)
-        return VideoM3U8(m3u8_video, m3u8_audio)
-
-    def get_segment_urls(
-        self,
-        base_url: str,
-        initialization_template_url: str,
-        segment_template_url: str,
-        end_time_millis: int,
-        segment_length: int,
-        profile_id: int,
-        file_type: str,
-    ) -> list[str]:
-        initialization_template_url_formated = initialization_template_url.replace(
-            "{{profile_id}}", str(profile_id)
-        ).replace("{{file_type}}", file_type)
-        segments = []
-        first_segment = base_url + initialization_template_url_formated
-        segments.append(first_segment)
-        for i in range(0, int(end_time_millis / 1000) + 1, segment_length):
-            segment_template_url_formated = (
-                segment_template_url.replace("{{profile_id}}", str(profile_id))
-                .replace("{{segment_timestamp}}", str(i))
-                .replace("{{file_type}}", file_type)
-            )
-            segments.append(base_url + segment_template_url_formated)
-        return segments
-
-    def save_m3u8(self, m3u8_str: str, m3u8_path: Path) -> None:
-        m3u8_path.parent.mkdir(parents=True, exist_ok=True)
-        m3u8_path.write_text(m3u8_str)
+    def get_file_id(self, metadata_gid: dict) -> str:
+        audio_files = metadata_gid.get("file")
+        if audio_files is None:
+            if metadata_gid.get("alternative") is not None:
+                audio_files = metadata_gid["alternative"][0]["file"]
+            else:
+                return None
+        return next(i["file_id"] for i in audio_files if i["format"] == self.codec)
 
     def get_tags(
         self,
         metadata_gid: dict,
         album_metadata: dict,
         track_credits: dict,
+        lyrics_unsynced: str,
     ) -> dict:
         isrc = None
         if metadata_gid.get("external_id"):
             isrc = next(
                 (i for i in metadata_gid["external_id"] if i["type"] == "isrc"), None
             )
         release_date_datetime_obj = self.downloader.get_release_date_datetime_obj(
@@ -220,109 +108,168 @@
         )["artists"]
         composers = next(
             role
             for role in track_credits["roleCredits"]
             if role["roleTitle"] == "Writers"
         )["artists"]
         tags = {
+            "album": album_metadata["name"],
+            "album_artist": self.downloader.get_artist(album_metadata["artists"]),
             "artist": self.downloader.get_artist(metadata_gid["artist"]),
+            "compilation": (
+                True if album_metadata["album_type"] == "compilation" else False
+            ),
             "composer": self.downloader.get_artist(composers) if composers else None,
             "copyright": next(
                 (i["text"] for i in album_metadata["copyrights"] if i["type"] == "P"),
                 None,
             ),
+            "disc": metadata_gid["disc_number"],
+            "disc_total": album_metadata["tracks"]["items"][-1]["disc_number"],
             "isrc": isrc.get("id") if isrc is not None else None,
-            "label": metadata_gid["album"].get("label"),
-            "media_type": 6,
+            "label": album_metadata.get("label"),
+            "lyrics": lyrics_unsynced,
+            "media_type": 1,
             "producer": self.downloader.get_artist(producers) if producers else None,
             "rating": 1 if metadata_gid.get("explicit") else 0,
-            "title": album_metadata["name"],
             "release_date": self.downloader.get_release_date_tag(
                 release_date_datetime_obj
             ),
+            "release_year": str(release_date_datetime_obj.year),
+            "title": metadata_gid["name"],
+            "track": metadata_gid["number"],
+            "track_total": max(
+                i["track_number"]
+                for i in album_metadata["tracks"]["items"]
+                if i["disc_number"] == metadata_gid["disc_number"]
+            ),
             "url": f"https://open.spotify.com/track/{self.downloader.spotify_api.gid_to_track_id(metadata_gid['gid'])}",
         }
-        tags["release_year"] = str(release_date_datetime_obj.year)
         return tags
 
-    def download(self, m3u8_path: Path, encrypted_path: str):
-        if self.download_mode == DownloadModeVideo.YTDLP:
-            self.download_ytdlp(m3u8_path, encrypted_path)
-        elif self.download_mode == DownloadModeVideo.NM3U8DLRE:
-            self.download_nm3u8dlre(m3u8_path, encrypted_path)
+    def download(self, encrypted_path: Path, stream_url: str):
+        if self.download_mode == DownloadModeSong.YTDLP:
+            self.download_ytdlp(encrypted_path, stream_url)
+        elif self.download_mode == DownloadModeSong.ARIA2C:
+            self.download_aria2c(encrypted_path, stream_url)
 
-    def download_ytdlp(self, m3u8_path: Path, encrypted_path: Path) -> None:
+    def download_ytdlp(self, encrypted_path: Path, stream_url: str) -> None:
         with YoutubeDL(
             {
                 "quiet": True,
                 "no_warnings": True,
                 "outtmpl": str(encrypted_path),
                 "allow_unplayable_formats": True,
                 "fixup": "never",
                 "allowed_extractors": ["generic"],
-                "noprogress": self.downloader.no_progress,
-                "enable_file_urls": True,
+                "noprogress": self.downloader.silence,
             }
         ) as ydl:
-            ydl.download(m3u8_path.resolve().as_uri())
+            ydl.download(stream_url)
 
-    def download_nm3u8dlre(self, m3u8_path: Path, encrypted_path: Path) -> None:
-        if self.downloader.no_progress:
-            subprocess_additional_args = {
-                "stdout": subprocess.DEVNULL,
-                "stderr": subprocess.DEVNULL,
-            }
-        else:
-            subprocess_additional_args = {}
+    def download_aria2c(self, encrypted_path: Path, stream_url: str) -> None:
         encrypted_path.parent.mkdir(parents=True, exist_ok=True)
         subprocess.run(
             [
-                self.downloader.nm3u8dlre_path_full,
-                m3u8_path,
-                "--binary-merge",
-                "--no-log",
-                "--log-level",
-                "off",
-                "--ffmpeg-binary-path",
-                self.downloader.ffmpeg_path_full,
-                "--save-name",
-                encrypted_path.stem,
-                "--save-dir",
-                encrypted_path.parent,
-                "--tmp-dir",
-                encrypted_path.parent,
+                self.downloader.aria2c_path_full,
+                "--no-conf",
+                "--download-result=hide",
+                "--console-log-level=error",
+                "--summary-interval=0",
+                "--file-allocation=none",
+                stream_url,
+                "--out",
+                encrypted_path,
+            ],
+            check=True,
+            **self.downloader.subprocess_additional_args,
+        )
+        print("\r", end="")
+
+    def remux(
+        self,
+        encrypted_path: Path,
+        decrypted_path: Path,
+        remuxed_path: Path,
+        decryption_key: str,
+    ):
+        if self.downloader.remux_mode == RemuxMode.FFMPEG:
+            self.remux_ffmpeg(decryption_key, encrypted_path, remuxed_path)
+        elif self.downloader.remux_mode == RemuxMode.MP4BOX:
+            self.downloader.decrypt_mp4decrypt(
+                encrypted_path, decrypted_path, decryption_key
+            )
+            self.remux_mp4box(decrypted_path, remuxed_path)
+
+    def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path):
+        subprocess.run(
+            [
+                self.downloader.mp4box_path_full,
+                "-quiet",
+                "-add",
+                decrypted_path,
+                "-itags",
+                "artist=placeholder",
+                "-keep-utc",
+                "-new",
+                remuxed_path,
             ],
             check=True,
-            **subprocess_additional_args,
+            **self.downloader.subprocess_additional_args,
         )
 
-    def fixup(
+    def remux_ffmpeg(
         self,
         decryption_key: str,
-        encrypted_path_video: Path,
-        encrypted_path_audio: Path,
+        encrypted_path: Path,
         fixed_path: Path,
     ) -> None:
         subprocess.run(
             [
                 self.downloader.ffmpeg_path_full,
                 "-loglevel",
                 "error",
                 "-y",
                 "-decryption_key",
                 decryption_key,
                 "-i",
-                encrypted_path_video,
-                "-decryption_key",
-                decryption_key,
-                "-i",
-                encrypted_path_audio,
-                "-c",
-                "copy",
+                encrypted_path,
                 "-movflags",
                 "+faststart",
-                "-fflags",
-                "+bitexact",
+                "-c",
+                "copy",
                 fixed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
+
+    def get_lyrics_synced_timestamp_lrc(self, time: int) -> str:
+        lrc_timestamp = datetime.datetime.fromtimestamp(
+            time / 1000.0, tz=datetime.timezone.utc
+        )
+        return lrc_timestamp.strftime("%M:%S.%f")[:-4]
+
+    def get_lyrics(self, track_id: str) -> Lyrics:
+        lyrics = Lyrics()
+        raw_lyrics = self.downloader.spotify_api.get_lyrics(track_id)
+        if raw_lyrics is None:
+            return lyrics
+        lyrics.synced = ""
+        lyrics.unsynced = ""
+        for line in raw_lyrics["lyrics"]["lines"]:
+            if raw_lyrics["lyrics"]["syncType"] == "LINE_SYNCED":
+                lyrics.synced += f'[{self.get_lyrics_synced_timestamp_lrc(int(line["startTimeMs"]))}]{line["words"]}\n'
+            lyrics.unsynced += f'{line["words"]}\n'
+        lyrics.unsynced = lyrics.unsynced[:-1]
+        return lyrics
+
+    def get_cover_path(self, final_path: Path) -> Path:
+        return final_path.parent / "Cover.jpg"
+
+    def get_lrc_path(self, final_path: Path) -> Path:
+        return final_path.with_suffix(".lrc")
+
+    def save_lrc(self, lrc_path: Path, lyrics_synced: str):
+        if lyrics_synced:
+            lrc_path.parent.mkdir(parents=True, exist_ok=True)
+            lrc_path.write_text(lyrics_synced, encoding="utf8")
```

### Comparing `spotify_web_downloader-1.6.6/spotify_web_downloader/hardcoded_wvd.py` & `spotify_web_downloader-1.6.7/spotify_web_downloader/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.6/spotify_web_downloader/models.py` & `spotify_web_downloader-1.6.7/spotify_web_downloader/models.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.6/spotify_web_downloader/spotify_api.py` & `spotify_web_downloader-1.6.7/spotify_web_downloader/spotify_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,15 @@
     PSSH_API_URL = "https://seektables.scdn.co/seektable/{file_id}.json"
     STREAM_URL_API_URL = (
         "https://gue1-spclient.spotify.com/storage-resolve/v2/files/audio/interactive/11/"
         "{file_id}?version=10000000&product=9&platform=39&alt=json"
     )
     METADATA_API_URL = "https://api.spotify.com/v1/{type}/{track_id}"
     PATHFINDER_API_URL = "https://api-partner.spotify.com/pathfinder/v1/query"
-    TRACK_CREDITS_API_URL = (
-        "https://spclient.wg.spotify.com/track-credits-view/v0/experimental/{track_id}/credits"
-    )
+    TRACK_CREDITS_API_URL = "https://spclient.wg.spotify.com/track-credits-view/v0/experimental/{track_id}/credits"
     EXTEND_TRACK_COLLECTION_WAIT_TIME = 0.5
 
     def __init__(
         self,
         cookies_path: Path = Path("./cookies.txt"),
     ):
         self.cookies_path = cookies_path
@@ -66,15 +64,17 @@
             {
                 "authorization": f"Bearer {token}",
             }
         )
 
     @staticmethod
     def _check_response(response: requests.Response):
-        if not response.ok:
+        try:
+            response.raise_for_status()
+        except requests.HTTPError:
             raise Exception(
                 f"Request failed with status code {response.status_code}: {response.text}"
             )
 
     @staticmethod
     def track_id_to_gid(track_id: str) -> str:
         return hex(base62.decode(track_id, base62.CHARSET_INVERTED))[2:].zfill(32)
```

### Comparing `spotify_web_downloader-1.6.6/PKG-INFO` & `spotify_web_downloader-1.6.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 Metadata-Version: 2.1
 Name: spotify-web-downloader
-Version: 1.6.6
-Summary: Download songs/albums/playlists directly from Spotify in AAC
+Version: 1.6.7
+Summary: A Python CLI app for downloading songs/music videos/albums/playlists directly from Spotify.
 Author: glomatico
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: pybase62
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: yt-dlp
 Project-URL: repository, https://github.com/glomatico/spotify-web-downloader
 
 # Spotify Web Downloader
-A Python script to download songs/music videos/albums/playlists directly from Spotify.
+A Python CLI app for downloading songs/music videos/albums/playlists directly from Spotify.
+
+**Discord Server:** https://discord.gg/aBjMEZ9tnq
 
 ## Features
-* Download songs in 128kbps AAC or in 256kbps AAC with a premium account
+* Download songs in AAC 128kbps or in AAC 256kbps with a premium account
 * Download music videos with a premium account
-* Download synced lyrics
+* Download synced lyrics with a premium account
 * Highly configurable
 
-## Pre-requisites
+## Prerequisites
+* Python 3.8 or higher
 * The cookies file of your Spotify account (free or premium)
-    * You can get your cookies by using this Google Chrome extension on Spotify website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
+    * You can get your cookies by using one of the following extensions on your browser of choice at the Spotify website with your account signed in:
+        * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
+        * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
 * FFmpeg on your system PATH
     * Older versions of FFmpeg may not work.
-* Python 3.7 or higher
+    * Up to date binaries can be obtained from the links below:
+        * Windows: https://github.com/AnimMouse/ffmpeg-stable-autobuild/releases
+        * Linux: https://johnvansickle.com/ffmpeg/
 
 ## Installation
 1. Install the package `spotify-web-downloader` using pip
     ```bash
     pip install spotify-web-downloader
     ```
-2. Place your cookies in the same directory you will run the script from and name it `cookies.txt`
+2. Place your cookies file in the directory from which you will be running spotify-web-downloader and name it `cookies.txt`.
 
 ## Usage
+```bash
+spotify-web-downloader [OPTIONS] URLS...
+```
+
+### Examples
 * Download a song
     ```bash
     spotify-web-downloader "https://open.spotify.com/track/18gqCQzqYb0zvurQPlRkpo"
     ```
 * Download an album
     ```bash
     spotify-web-downloader "https://open.spotify.com/album/0r8D5N674HbTXlR3zNxeU1"
@@ -59,30 +71,34 @@
 | `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
 | `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
 | `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
 | `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Spotify`                                  |
 | `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
 | `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
 | `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
 | `--aria2c-path` / `aria2c_path`                                 | Path to aria2c binary.                                                       | `aria2c`                                     |
 | `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8DL-RE`                                |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
 | `--date-tag-template` / `date_tag_template`                     | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
 | `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
 | `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
 | `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                            | `{album_artist}/{album}`                     |
 | `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.                | `Compilations/{album}`                       |
 | `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string.        | `{track:02d} {title}`                        |
 | `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.         | `{disc}-{track:02d} {title}`                 |
 | `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ytdlp`                                      |
 | `--premium-quality`, `-p` / `premium_quality`                   | Download songs in premium quality.                                           | `false`                                      |
 | `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                      | `{artist}/Unknown Album`                     |
 | `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                        | `{title}`                                    |
-| `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ydlp`                                       |
+| `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ytdlp`                                      |
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
+
 ### Tag variables
 The following variables can be used in the template folder/file and/or in the `exclude_tags` list:
 - `album`
 - `album_artist`
 - `artist`
 - `compilation`
 - `composer`
@@ -98,19 +114,26 @@
 - `rating`
 - `release_date`
 - `release_year`
 - `title`
 - `track`
 - `track_total`
 - `url`
+  
+### Remux modes
+The following remux modes are available:
+* `ffmpeg`
+* `mp4box`
+    * Requires mp4decrypt
+    * Can be obtained from here: https://gpac.wp.imt.fr/downloads
 
 ### Music videos quality
 Music videos will be downloaded in the highest quality available in H.264/AAC, up to 1080p.
 
-### Download mode
+### Download modes
 The following modes are available for songs:
 * `ytdlp`
 * `aria2c`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/aria2/aria2/releases
 
 The following modes are available for videos:
```

