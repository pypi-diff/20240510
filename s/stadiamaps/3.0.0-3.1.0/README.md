# Comparing `tmp/stadiamaps-3.0.0.tar.gz` & `tmp/stadiamaps-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadiamaps-3.0.0.tar", last modified: Tue Apr 30 07:04:56 2024, max compression
+gzip compressed data, was "stadiamaps-3.1.0.tar", last modified: Fri May 10 19:27:24 2024, max compression
```

## Comparing `stadiamaps-3.0.0.tar` & `stadiamaps-3.1.0.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.947810 stadiamaps-3.0.0/stadiamaps/
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.951810 stadiamaps-3.0.0/stadiamaps/api/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   147742 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29289 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    80984 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/routing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25932 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.971810 stadiamaps-3.0.0/stadiamaps/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/admin_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/administrative.py
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/bike_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/directions_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/edge_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/end_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/height_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/height_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/low_speed_vehicle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matched_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/node_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/road_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_leg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_response_alternates_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/speeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/traversability.py
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/tz_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/warning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/stadiamaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_eu_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_gecoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_geospatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_admin_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_administrative.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_bike_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_directions_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_edge_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_end_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_height_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_height_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_low_speed_vehicle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matched_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_node_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_road_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_leg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_response_alternates_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_speeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_traversability.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_tz_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.149808 stadiamaps-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-10 19:27:24.149808 stadiamaps-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 19:27:24.149808 stadiamaps-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.109808 stadiamaps-3.1.0/stadiamaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.113808 stadiamaps-3.1.0/stadiamaps/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147812 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/api/geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29317 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/api/geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80146 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/api/routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26365 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.129808 stadiamaps-3.1.0/stadiamaps/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/administrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/end_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/height_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/height_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/low_speed_vehicle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/matrix_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/node_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/road_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_response_alternates_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/route_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/speeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/traversability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/models/warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/stadiamaps/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.149808 stadiamaps-3.1.0/stadiamaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-10 19:27:24.000000 stadiamaps-3.1.0/stadiamaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-10 19:27:24.000000 stadiamaps-3.1.0/stadiamaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:27:24.000000 stadiamaps-3.1.0/stadiamaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 19:27:24.000000 stadiamaps-3.1.0/stadiamaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 19:27:24.000000 stadiamaps-3.1.0/stadiamaps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.149808 stadiamaps-3.1.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:24.149808 stadiamaps-3.1.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/integration/test_eu_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/integration/test_gecoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/integration/test_geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/integration/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_administrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_end_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_height_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_height_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_low_speed_vehicle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_matrix_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_road_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_response_alternates_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_route_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_speeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_traversability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-10 19:27:19.000000 stadiamaps-3.1.0/test/test_warning.py
```

### Comparing `stadiamaps-3.0.0/LICENSE.txt` & `stadiamaps-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/PKG-INFO` & `stadiamaps-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 3.0.0
+Version: 3.1.0
 Summary: Stadia Maps Geospatial APIs
 Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-3.0.0/README.md` & `stadiamaps-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/pyproject.toml` & `stadiamaps-3.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stadiamaps"
-version = "3.0.0"
+version = "3.1.0"
 description = "Stadia Maps Geospatial APIs"
 authors = ["Stadia Maps Support <support@stadiamaps.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/stadiamaps/stadiamaps-api-py"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Stadia Maps Geospatial APIs"]
 include = ["stadiamaps/py.typed"]
```

### Comparing `stadiamaps-3.0.0/setup.py` & `stadiamaps-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "stadiamaps"
-VERSION = "3.0.0"
+VERSION = "3.1.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `stadiamaps-3.0.0/stadiamaps/__init__.py` & `stadiamaps-3.1.0/stadiamaps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 # import apis into sdk package
 from stadiamaps.api.geocoding_api import GeocodingApi
 from stadiamaps.api.geospatial_api import GeospatialApi
 from stadiamaps.api.routing_api import RoutingApi
 
 # import ApiClient
```

### Comparing `stadiamaps-3.0.0/stadiamaps/api/geocoding_api.py` & `stadiamaps-3.1.0/stadiamaps/api/geocoding_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,15 +454,15 @@
             'sources': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if text is not None:
             
             _query_params.append(('text', text))
@@ -791,15 +791,15 @@
             'ids': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if ids is not None:
             
             _query_params.append(('ids', ids))
@@ -1165,15 +1165,15 @@
             'boundary.country': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if point_lat is not None:
             
             _query_params.append(('point.lat', point_lat))
@@ -1658,15 +1658,15 @@
             'sources': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if text is not None:
             
             _query_params.append(('text', text))
@@ -2270,15 +2270,15 @@
             'sources': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if address is not None:
             
             _query_params.append(('address', address))
```

### Comparing `stadiamaps-3.0.0/stadiamaps/api/geospatial_api.py` & `stadiamaps-3.1.0/stadiamaps/api/geospatial_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -556,15 +556,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if lat is not None:
             
             _query_params.append(('lat', lat))
```

### Comparing `stadiamaps-3.0.0/stadiamaps/api/routing_api.py` & `stadiamaps-3.1.0/stadiamaps/api/routing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from typing import Optional
+from typing import List, Optional
 from stadiamaps.models.isochrone_request import IsochroneRequest
 from stadiamaps.models.isochrone_response import IsochroneResponse
 from stadiamaps.models.locate_object import LocateObject
 from stadiamaps.models.map_match_request import MapMatchRequest
 from stadiamaps.models.map_match_route_response import MapMatchRouteResponse
 from stadiamaps.models.matrix_request import MatrixRequest
 from stadiamaps.models.matrix_response import MatrixResponse
@@ -264,15 +264,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -541,15 +541,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -815,15 +815,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1092,15 +1092,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1369,15 +1369,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1444,15 +1444,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> MatrixResponse:
         """Calculate a time distance matrix for use in an optimizer.
 
-        The time distance matrix API lets you compare travel times between a set of possible start and end points. Note that this endpoint has a limit of 22,500 elements, regardless of the costing/mode of travel. A matrix request with 3 inputs and 5 outputs has 3 x 5 = 15 elements. For example, a matrix request with 3 inputs and 5 outputs has 3 x 5 = 15 elements. This means you could send a 150 x 150 or 30 x 750 matrix request (each having 22,500 elements), but not a 500 x 500 matrix (250,000 elements).
+        The time distance matrix API lets you compare travel times between a set of possible start and end points. See https://docs.stadiamaps.com/limits/ for documentation of our latest limits.
 
         :param matrix_request:
         :type matrix_request: MatrixRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1512,15 +1512,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[MatrixResponse]:
         """Calculate a time distance matrix for use in an optimizer.
 
-        The time distance matrix API lets you compare travel times between a set of possible start and end points. Note that this endpoint has a limit of 22,500 elements, regardless of the costing/mode of travel. A matrix request with 3 inputs and 5 outputs has 3 x 5 = 15 elements. For example, a matrix request with 3 inputs and 5 outputs has 3 x 5 = 15 elements. This means you could send a 150 x 150 or 30 x 750 matrix request (each having 22,500 elements), but not a 500 x 500 matrix (250,000 elements).
+        The time distance matrix API lets you compare travel times between a set of possible start and end points. See https://docs.stadiamaps.com/limits/ for documentation of our latest limits.
 
         :param matrix_request:
         :type matrix_request: MatrixRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1580,15 +1580,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Calculate a time distance matrix for use in an optimizer.
 
-        The time distance matrix API lets you compare travel times between a set of possible start and end points. Note that this endpoint has a limit of 22,500 elements, regardless of the costing/mode of travel. A matrix request with 3 inputs and 5 outputs has 3 x 5 = 15 elements. For example, a matrix request with 3 inputs and 5 outputs has 3 x 5 = 15 elements. This means you could send a 150 x 150 or 30 x 750 matrix request (each having 22,500 elements), but not a 500 x 500 matrix (250,000 elements).
+        The time distance matrix API lets you compare travel times between a set of possible start and end points. See https://docs.stadiamaps.com/limits/ for documentation of our latest limits.
 
         :param matrix_request:
         :type matrix_request: MatrixRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1643,15 +1643,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1917,15 +1917,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `stadiamaps-3.0.0/stadiamaps/api_client.py` & `stadiamaps-3.1.0/stadiamaps/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
-from typing import Tuple, Optional, List, Dict
+from typing import Tuple, Optional, List, Dict, Union
+from pydantic import SecretStr
 
 from stadiamaps.configuration import Configuration
 from stadiamaps.api_response import ApiResponse, T as ApiResponseT
 import stadiamaps.models
 from stadiamaps import rest
 from stadiamaps.exceptions import (
     ApiValueError,
@@ -84,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
@@ -204,15 +205,16 @@
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(
                 post_params,
                 collection_formats
             )
-            post_params.extend(self.files_parameters(files))
+            if files:
+                post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(
             header_params,
             query_params,
             auth_settings,
             resource_path,
@@ -309,15 +311,18 @@
             elif response_type is not None:
                 match = None
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
                 encoding = match.group(1) if match else "utf-8"
                 response_text = response_data.data.decode(encoding)
-                return_data = self.deserialize(response_text, response_type)
+                if response_type in ["bytearray", "str"]:
+                    return_data = self.__deserialize_primitive(response_text, response_type)
+                else:
+                    return_data = self.deserialize(response_text, response_type)
         finally:
             if not 200 <= response_data.status <= 299:
                 raise ApiException.from_response(
                     http_resp=response_data,
                     body=response_text,
                     data=return_data,
                 )
@@ -329,26 +334,31 @@
             raw_data = response_data.data
         )
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
+        If obj is SecretStr, return obj.get_secret_value()
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
 
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
+        elif isinstance(obj, Enum):
+            return obj.value
+        elif isinstance(obj, SecretStr):
+            return obj.get_secret_value()
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
             return [
                 self.sanitize_for_serialization(sub_obj) for sub_obj in obj
             ]
         elif isinstance(obj, tuple):
@@ -362,15 +372,18 @@
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
-            obj_dict = obj.to_dict()
+            if hasattr(obj, 'to_dict') and callable(getattr(obj, 'to_dict')):
+                obj_dict = obj.to_dict()
+            else:
+                obj_dict = obj.__dict__
 
         return {
             key: self.sanitize_for_serialization(val)
             for key, val in obj_dict.items()
         }
 
     def deserialize(self, response_text, response_type):
@@ -477,16 +490,14 @@
         if collection_formats is None:
             collection_formats = {}
         for k, v in params.items() if isinstance(params, dict) else params:
             if isinstance(v, bool):
                 v = str(v).lower()
             if isinstance(v, (int, float)):
                 v = str(v)
-            if isinstance(v, Enum):
-                v = str(v.value)
             if isinstance(v, dict):
                 v = json.dumps(v)
 
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
                     new_params.extend((k, str(value)) for value in v)
@@ -496,46 +507,45 @@
                     elif collection_format == 'tsv':
                         delimiter = '\t'
                     elif collection_format == 'pipes':
                         delimiter = '|'
                     else:  # csv is the default
                         delimiter = ','
                     new_params.append(
-                        (k, delimiter.join(quote(str(value.value) if isinstance(value, Enum) else str(value)) for value in v))
+                        (k, delimiter.join(quote(str(value)) for value in v))
                     )
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(map(str, item)) for item in new_params])
 
-    def files_parameters(self, files=None):
+    def files_parameters(self, files: Dict[str, Union[str, bytes]]):
         """Builds form parameters.
 
         :param files: File parameters.
         :return: Form parameters with files.
         """
         params = []
-
-        if files:
-            for k, v in files.items():
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (
-                            mimetypes.guess_type(filename)[0]
-                            or 'application/octet-stream'
-                        )
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])])
-                        )
-
+        for k, v in files.items():
+            if isinstance(v, str):
+                with open(v, 'rb') as f:
+                    filename = os.path.basename(f.name)
+                    filedata = f.read()
+            elif isinstance(v, bytes):
+                filename = k
+                filedata = v
+            else:
+                raise ValueError("Unsupported file value")
+            mimetype = (
+                mimetypes.guess_type(filename)[0]
+                or 'application/octet-stream'
+            )
+            params.append(
+                tuple([k, tuple([filename, filedata, mimetype])])
+            )
         return params
 
     def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
```

### Comparing `stadiamaps-3.0.0/stadiamaps/api_response.py` & `stadiamaps-3.1.0/stadiamaps/api_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/configuration.py` & `stadiamaps-3.1.0/stadiamaps/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 6.3.0\n"\
-               "SDK Package Version: 3.0.0".\
+               "SDK Package Version: 3.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `stadiamaps-3.0.0/stadiamaps/exceptions.py` & `stadiamaps-3.1.0/stadiamaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/__init__.py` & `stadiamaps-3.1.0/stadiamaps/models/__init__.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/access.py` & `stadiamaps-3.1.0/stadiamaps/models/access.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/admin_region.py` & `stadiamaps-3.1.0/stadiamaps/models/admin_region.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/administrative.py` & `stadiamaps-3.1.0/stadiamaps/models/administrative.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/auto_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/auto_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/auto_costing_options_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/base_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/base_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/base_trace_request.py` & `stadiamaps-3.1.0/stadiamaps/models/base_trace_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/bicycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/bike_network.py` & `stadiamaps-3.1.0/stadiamaps/models/bike_network.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/contour.py` & `stadiamaps-3.1.0/stadiamaps/models/contour.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/coordinate.py` & `stadiamaps-3.1.0/stadiamaps/models/coordinate.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/costing_model.py` & `stadiamaps-3.1.0/stadiamaps/models/costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/directions_options.py` & `stadiamaps-3.1.0/stadiamaps/models/directions_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/distance_unit.py` & `stadiamaps-3.1.0/stadiamaps/models/distance_unit.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/edge_sign.py` & `stadiamaps-3.1.0/stadiamaps/models/edge_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/edge_use.py` & `stadiamaps-3.1.0/stadiamaps/models/edge_use.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/end_node.py` & `stadiamaps-3.1.0/stadiamaps/models/end_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_attributes.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_attributes.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import pprint
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
 from typing import Any, List, Optional
 from stadiamaps.models.geo_json_line_string import GeoJSONLineString
 from stadiamaps.models.geo_json_point import GeoJSONPoint
 from stadiamaps.models.geo_json_polygon import GeoJSONPolygon
 from pydantic import StrictStr, Field
-from typing import Union, List, Optional, Dict
+from typing import Union, List, Set, Optional, Dict
 from typing_extensions import Literal, Self
 
 GEOJSONGEOMETRY_ONE_OF_SCHEMAS = ["GeoJSONLineString", "GeoJSONPoint", "GeoJSONPolygon"]
 
 class GeoJSONGeometry(BaseModel):
     """
     GeoJSONGeometry
@@ -34,15 +34,15 @@
     # data type: GeoJSONPoint
     oneof_schema_1_validator: Optional[GeoJSONPoint] = None
     # data type: GeoJSONLineString
     oneof_schema_2_validator: Optional[GeoJSONLineString] = None
     # data type: GeoJSONPolygon
     oneof_schema_3_validator: Optional[GeoJSONPolygon] = None
     actual_instance: Optional[Union[GeoJSONLineString, GeoJSONPoint, GeoJSONPolygon]] = None
-    one_of_schemas: List[str] = Field(default=Literal["GeoJSONLineString", "GeoJSONPoint", "GeoJSONPolygon"])
+    one_of_schemas: Set[str] = { "GeoJSONLineString", "GeoJSONPoint", "GeoJSONPolygon" }
 
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
     )
```

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry_base.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_geometry_base.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_line_string.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_point.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_point_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_polygon.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/geocoding_object.py` & `stadiamaps-3.1.0/stadiamaps/models/geocoding_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/height_request.py` & `stadiamaps-3.1.0/stadiamaps/models/height_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/height_response.py` & `stadiamaps-3.1.0/stadiamaps/models/height_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/highway_classification.py` & `stadiamaps-3.1.0/stadiamaps/models/highway_classification.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/intersecting_edge.py` & `stadiamaps-3.1.0/stadiamaps/models/intersecting_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/isochrone_costing_model.py` & `stadiamaps-3.1.0/stadiamaps/models/isochrone_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/isochrone_feature.py` & `stadiamaps-3.1.0/stadiamaps/models/isochrone_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/isochrone_properties.py` & `stadiamaps-3.1.0/stadiamaps/models/isochrone_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/isochrone_request.py` & `stadiamaps-3.1.0/stadiamaps/models/isochrone_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/isochrone_response.py` & `stadiamaps-3.1.0/stadiamaps/models/isochrone_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/locate_detailed_edge.py` & `stadiamaps-3.1.0/stadiamaps/models/locate_detailed_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/locate_edge.py` & `stadiamaps-3.1.0/stadiamaps/models/locate_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/locate_edge_info.py` & `stadiamaps-3.1.0/stadiamaps/models/locate_edge_info.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/locate_node.py` & `stadiamaps-3.1.0/stadiamaps/models/locate_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/locate_node_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/locate_object.py` & `stadiamaps-3.1.0/stadiamaps/models/locate_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/low_speed_vehicle_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/low_speed_vehicle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/maneuver_sign.py` & `stadiamaps-3.1.0/stadiamaps/models/maneuver_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/maneuver_sign_element.py` & `stadiamaps-3.1.0/stadiamaps/models/maneuver_sign_element.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_costing_model.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_request.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_request_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_route_response.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_route_response_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_trace_options.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_trace_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/matched_point.py` & `stadiamaps-3.1.0/stadiamaps/models/matched_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/matrix_costing_model.py` & `stadiamaps-3.1.0/stadiamaps/models/matrix_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/matrix_distance.py` & `stadiamaps-3.1.0/stadiamaps/models/matrix_distance.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/matrix_request.py` & `stadiamaps-3.1.0/stadiamaps/models/matrix_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/matrix_response.py` & `stadiamaps-3.1.0/stadiamaps/models/matrix_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from typing_extensions import Self
 
 class MatrixResponse(BaseModel):
     """
     MatrixResponse
     """ # noqa: E501
     id: Optional[StrictStr] = Field(default=None, description="An identifier to disambiguate requests (echoed by the server).")
-    sources: Annotated[List[Coordinate], Field(min_length=1)] = Field(description="The list of starting locations")
-    targets: Annotated[List[Coordinate], Field(min_length=1)] = Field(description="The list of ending locations")
+    sources: Annotated[List[Coordinate], Field(min_length=1)] = Field(description="The list of starting locations determined by snapping to the nearest appropriate point on the road network for the costing model. All locations appear in the same order as the input.")
+    targets: Annotated[List[Coordinate], Field(min_length=1)] = Field(description="The list of ending locations determined by snapping to the nearest appropriate point on the road network for the costing model. All locations appear in the same order as the input.")
     sources_to_targets: Annotated[List[List[MatrixDistance]], Field(min_length=1)] = Field(description="The matrix of starting and ending locations, along with the computed distance and travel time. The array is row-ordered. This means that the time and distance from the first location to all others forms the first row of the array, followed by the time and distance from the second source location to all target locations, etc.")
     warnings: Optional[List[Warning]] = None
     units: ValhallaLongUnits
     additional_properties: Dict[str, Any] = {}
     __properties: ClassVar[List[str]] = ["id", "sources", "targets", "sources_to_targets", "warnings", "units"]
 
     model_config = ConfigDict(
```

### Comparing `stadiamaps-3.0.0/stadiamaps/models/matrix_waypoint.py` & `stadiamaps-3.1.0/stadiamaps/models/matrix_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/motor_scooter_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/motorcycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/nearest_roads_request.py` & `stadiamaps-3.1.0/stadiamaps/models/nearest_roads_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/node_id.py` & `stadiamaps-3.1.0/stadiamaps/models/node_id.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/node_type.py` & `stadiamaps-3.1.0/stadiamaps/models/node_type.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/optimized_route_request.py` & `stadiamaps-3.1.0/stadiamaps/models/optimized_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pedestrian_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/pedestrian_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_feature.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_properties_addendum.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_layer.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_layer.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_response.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_response_geocoding.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/pelias_source.py` & `stadiamaps-3.1.0/stadiamaps/models/pelias_source.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/restrictions.py` & `stadiamaps-3.1.0/stadiamaps/models/restrictions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/road_class.py` & `stadiamaps-3.1.0/stadiamaps/models/road_class.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_leg.py` & `stadiamaps-3.1.0/stadiamaps/models/route_trip.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,31 +14,37 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List
-from typing_extensions import Annotated
-from stadiamaps.models.route_maneuver import RouteManeuver
+from stadiamaps.models.route_leg import RouteLeg
 from stadiamaps.models.route_summary import RouteSummary
+from stadiamaps.models.routing_response_waypoint import RoutingResponseWaypoint
+from stadiamaps.models.valhalla_languages import ValhallaLanguages
+from stadiamaps.models.valhalla_long_units import ValhallaLongUnits
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RouteLeg(BaseModel):
+class RouteTrip(BaseModel):
     """
-    RouteLeg
+    RouteTrip
     """ # noqa: E501
-    maneuvers: Annotated[List[RouteManeuver], Field(min_length=1)]
-    shape: StrictStr = Field(description="An encoded polyline (https://developers.google.com/maps/documentation/utilities/polylinealgorithm) with 6 digits of decimal precision.")
+    status: StrictInt = Field(description="The response status code")
+    status_message: StrictStr = Field(description="The response status message")
+    units: ValhallaLongUnits
+    language: ValhallaLanguages
+    locations: List[RoutingResponseWaypoint]
+    legs: List[RouteLeg]
     summary: RouteSummary
     additional_properties: Dict[str, Any] = {}
-    __properties: ClassVar[List[str]] = ["maneuvers", "shape", "summary"]
+    __properties: ClassVar[List[str]] = ["status", "status_message", "units", "language", "locations", "legs", "summary"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -50,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RouteLeg from a JSON string"""
+        """Create an instance of RouteTrip from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,43 +79,54 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in maneuvers (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in locations (list)
         _items = []
-        if self.maneuvers:
-            for _item in self.maneuvers:
+        if self.locations:
+            for _item in self.locations:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['maneuvers'] = _items
+            _dict['locations'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in legs (list)
+        _items = []
+        if self.legs:
+            for _item in self.legs:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['legs'] = _items
         # override the default output from pydantic by calling `to_dict()` of summary
         if self.summary:
             _dict['summary'] = self.summary.to_dict()
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RouteLeg from a dict"""
+        """Create an instance of RouteTrip from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "maneuvers": [RouteManeuver.from_dict(_item) for _item in obj["maneuvers"]] if obj.get("maneuvers") is not None else None,
-            "shape": obj.get("shape"),
+            "status": obj.get("status"),
+            "status_message": obj.get("status_message"),
+            "units": obj.get("units"),
+            "language": obj.get("language"),
+            "locations": [RoutingResponseWaypoint.from_dict(_item) for _item in obj["locations"]] if obj.get("locations") is not None else None,
+            "legs": [RouteLeg.from_dict(_item) for _item in obj["legs"]] if obj.get("legs") is not None else None,
             "summary": RouteSummary.from_dict(obj["summary"]) if obj.get("summary") is not None else None
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
```

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_maneuver.py` & `stadiamaps-3.1.0/stadiamaps/models/route_maneuver.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_request.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attributes_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,41 +14,51 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from typing_extensions import Annotated
-from stadiamaps.models.costing_model import CostingModel
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
 from stadiamaps.models.costing_options import CostingOptions
 from stadiamaps.models.distance_unit import DistanceUnit
-from stadiamaps.models.routing_waypoint import RoutingWaypoint
+from stadiamaps.models.map_match_costing_model import MapMatchCostingModel
+from stadiamaps.models.map_match_waypoint import MapMatchWaypoint
+from stadiamaps.models.trace_attribute_filter_options import TraceAttributeFilterOptions
 from stadiamaps.models.valhalla_languages import ValhallaLanguages
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RouteRequest(BaseModel):
+class TraceAttributesRequest(BaseModel):
     """
-    RouteRequest
+    TraceAttributesRequest
     """ # noqa: E501
+    id: Optional[StrictStr] = Field(default=None, description="An identifier to disambiguate requests (echoed by the server).")
+    shape: Optional[List[MapMatchWaypoint]] = Field(default=None, description="REQUIRED if `encoded_polyline` is not present. Note that `break` type locations are only supported when `shape_match` is set to `map_match`.")
+    encoded_polyline: Optional[StrictStr] = Field(default=None, description="REQUIRED if `shape` is not present. An encoded polyline (https://developers.google.com/maps/documentation/utilities/polylinealgorithm). Note that the polyline must be encoded with 6 digits of precision rather than the usual 5.")
+    costing: MapMatchCostingModel
+    costing_options: Optional[CostingOptions] = None
+    shape_match: Optional[StrictStr] = Field(default=None, description="Three snapping modes provide some control over how the map matching occurs. `edge_walk` is fast, but requires extremely precise data that matches the route graph almost perfectly. `map_snap` can handle significantly noisier data, but is very expensive. `walk_or_snap`, the default, tries to use edge walking first and falls back to map matching if edge walking fails. In general, you should not need to change this parameter unless you want to trace a multi-leg route with multiple `break` locations in the `shape`.")
     units: Optional[DistanceUnit] = None
     language: Optional[ValhallaLanguages] = None
     directions_type: Optional[StrictStr] = Field(default='instructions', description="The level of directional narrative to include. Locations and times will always be returned, but narrative generation verbosity can be controlled with this parameter.")
-    id: Optional[StrictStr] = Field(default=None, description="An identifier to disambiguate requests (echoed by the server).")
-    locations: Annotated[List[RoutingWaypoint], Field(min_length=2)]
-    costing: CostingModel
-    costing_options: Optional[CostingOptions] = None
-    exclude_locations: Optional[List[RoutingWaypoint]] = Field(default=None, description="This has the same format as the locations list. Locations are mapped to the closed road(s), and these road(s) are excluded from the route path computation.")
-    exclude_polygons: Optional[List[List[List[Union[StrictFloat, StrictInt]]]]] = Field(default=None, description="One or multiple exterior rings of polygons in the form of nested JSON arrays. Roads intersecting these rings will be avoided during path finding. Open rings will be closed automatically. If you only need to avoid a few specific roads, it's much more efficient to use `exclude_locations`.")
-    alternates: Optional[StrictInt] = Field(default=None, description="How many alternate routes are desired. Note that fewer or no alternates may be returned. Alternates are not yet supported on routes with more than 2 locations or on time-dependent routes.")
+    filters: Optional[TraceAttributeFilterOptions] = Field(default=None, description="If present, provides either a whitelist or a blacklist of keys to include/exclude in the response. This key is optional, and if omitted from the request, all available info will be returned.")
     additional_properties: Dict[str, Any] = {}
-    __properties: ClassVar[List[str]] = ["units", "language", "directions_type", "id", "locations", "costing", "costing_options", "exclude_locations", "exclude_polygons", "alternates"]
+    __properties: ClassVar[List[str]] = ["id", "shape", "encoded_polyline", "costing", "costing_options", "shape_match", "units", "language", "directions_type", "filters"]
+
+    @field_validator('shape_match')
+    def shape_match_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['edge_walk', 'map_snap', 'walk_or_snap']):
+            raise ValueError("must be one of enum values ('edge_walk', 'map_snap', 'walk_or_snap')")
+        return value
 
     @field_validator('directions_type')
     def directions_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -70,15 +80,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RouteRequest from a JSON string"""
+        """Create an instance of TraceAttributesRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -93,58 +103,54 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in locations (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in shape (list)
         _items = []
-        if self.locations:
-            for _item in self.locations:
+        if self.shape:
+            for _item in self.shape:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['locations'] = _items
+            _dict['shape'] = _items
         # override the default output from pydantic by calling `to_dict()` of costing_options
         if self.costing_options:
             _dict['costing_options'] = self.costing_options.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in exclude_locations (list)
-        _items = []
-        if self.exclude_locations:
-            for _item in self.exclude_locations:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['exclude_locations'] = _items
+        # override the default output from pydantic by calling `to_dict()` of filters
+        if self.filters:
+            _dict['filters'] = self.filters.to_dict()
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RouteRequest from a dict"""
+        """Create an instance of TraceAttributesRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "units": obj.get("units"),
-            "language": obj.get("language"),
-            "directions_type": obj.get("directions_type") if obj.get("directions_type") is not None else 'instructions',
             "id": obj.get("id"),
-            "locations": [RoutingWaypoint.from_dict(_item) for _item in obj["locations"]] if obj.get("locations") is not None else None,
+            "shape": [MapMatchWaypoint.from_dict(_item) for _item in obj["shape"]] if obj.get("shape") is not None else None,
+            "encoded_polyline": obj.get("encoded_polyline"),
             "costing": obj.get("costing"),
             "costing_options": CostingOptions.from_dict(obj["costing_options"]) if obj.get("costing_options") is not None else None,
-            "exclude_locations": [RoutingWaypoint.from_dict(_item) for _item in obj["exclude_locations"]] if obj.get("exclude_locations") is not None else None,
-            "exclude_polygons": obj.get("exclude_polygons"),
-            "alternates": obj.get("alternates")
+            "shape_match": obj.get("shape_match"),
+            "units": obj.get("units"),
+            "language": obj.get("language"),
+            "directions_type": obj.get("directions_type") if obj.get("directions_type") is not None else 'instructions',
+            "filters": TraceAttributeFilterOptions.from_dict(obj["filters"]) if obj.get("filters") is not None else None
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
 
         return _obj
```

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_response.py` & `stadiamaps-3.1.0/stadiamaps/models/route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_response_alternates_inner.py` & `stadiamaps-3.1.0/stadiamaps/models/route_response_alternates_inner.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_response_trip.py` & `stadiamaps-3.1.0/stadiamaps/models/route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_summary.py` & `stadiamaps-3.1.0/stadiamaps/models/route_summary.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/route_trip.py` & `stadiamaps-3.1.0/stadiamaps/models/route_leg.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,37 +14,33 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List
-from stadiamaps.models.route_leg import RouteLeg
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing_extensions import Annotated
+from stadiamaps.models.route_maneuver import RouteManeuver
 from stadiamaps.models.route_summary import RouteSummary
-from stadiamaps.models.routing_response_waypoint import RoutingResponseWaypoint
-from stadiamaps.models.valhalla_languages import ValhallaLanguages
-from stadiamaps.models.valhalla_long_units import ValhallaLongUnits
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RouteTrip(BaseModel):
+class RouteLeg(BaseModel):
     """
-    RouteTrip
+    RouteLeg
     """ # noqa: E501
-    status: StrictInt = Field(description="The response status code")
-    status_message: StrictStr = Field(description="The response status message")
-    units: ValhallaLongUnits
-    language: ValhallaLanguages
-    locations: List[RoutingResponseWaypoint]
-    legs: List[RouteLeg]
+    maneuvers: Annotated[List[RouteManeuver], Field(min_length=1)]
+    shape: StrictStr = Field(description="An encoded polyline (https://developers.google.com/maps/documentation/utilities/polylinealgorithm) with 6 digits of decimal precision.")
     summary: RouteSummary
+    elevation_interval: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="The sampling distance between elevation values along the route. This echoes the request parameter having the same name.")
+    elevation: Optional[List[Union[StrictFloat, StrictInt]]] = Field(default=None, description="An array of elevation values sampled every `elevation_interval`. Units are either metric or imperial depending on the value of `units`.")
     additional_properties: Dict[str, Any] = {}
-    __properties: ClassVar[List[str]] = ["status", "status_message", "units", "language", "locations", "legs", "summary"]
+    __properties: ClassVar[List[str]] = ["maneuvers", "shape", "summary", "elevation_interval", "elevation"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -56,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RouteTrip from a JSON string"""
+        """Create an instance of RouteLeg from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,55 +75,46 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in locations (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in maneuvers (list)
         _items = []
-        if self.locations:
-            for _item in self.locations:
+        if self.maneuvers:
+            for _item in self.maneuvers:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['locations'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in legs (list)
-        _items = []
-        if self.legs:
-            for _item in self.legs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['legs'] = _items
+            _dict['maneuvers'] = _items
         # override the default output from pydantic by calling `to_dict()` of summary
         if self.summary:
             _dict['summary'] = self.summary.to_dict()
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RouteTrip from a dict"""
+        """Create an instance of RouteLeg from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status"),
-            "status_message": obj.get("status_message"),
-            "units": obj.get("units"),
-            "language": obj.get("language"),
-            "locations": [RoutingResponseWaypoint.from_dict(_item) for _item in obj["locations"]] if obj.get("locations") is not None else None,
-            "legs": [RouteLeg.from_dict(_item) for _item in obj["legs"]] if obj.get("legs") is not None else None,
-            "summary": RouteSummary.from_dict(obj["summary"]) if obj.get("summary") is not None else None
+            "maneuvers": [RouteManeuver.from_dict(_item) for _item in obj["maneuvers"]] if obj.get("maneuvers") is not None else None,
+            "shape": obj.get("shape"),
+            "summary": RouteSummary.from_dict(obj["summary"]) if obj.get("summary") is not None else None,
+            "elevation_interval": obj.get("elevation_interval"),
+            "elevation": obj.get("elevation")
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
 
         return _obj
```

### Comparing `stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint.py` & `stadiamaps-3.1.0/stadiamaps/models/routing_response_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/routing_waypoint.py` & `stadiamaps-3.1.0/stadiamaps/models/routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py` & `stadiamaps-3.1.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint.py` & `stadiamaps-3.1.0/stadiamaps/models/simple_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/speeds.py` & `stadiamaps-3.1.0/stadiamaps/models/speeds.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attribute_filter_options.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attribute_filter_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attribute_key.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attribute_key.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_base_response.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attributes_base_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request.py` & `stadiamaps-3.1.0/stadiamaps/models/route_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,51 +14,43 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing_extensions import Annotated
+from stadiamaps.models.costing_model import CostingModel
 from stadiamaps.models.costing_options import CostingOptions
 from stadiamaps.models.distance_unit import DistanceUnit
-from stadiamaps.models.map_match_costing_model import MapMatchCostingModel
-from stadiamaps.models.map_match_waypoint import MapMatchWaypoint
-from stadiamaps.models.trace_attribute_filter_options import TraceAttributeFilterOptions
+from stadiamaps.models.routing_waypoint import RoutingWaypoint
 from stadiamaps.models.valhalla_languages import ValhallaLanguages
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TraceAttributesRequest(BaseModel):
+class RouteRequest(BaseModel):
     """
-    TraceAttributesRequest
+    RouteRequest
     """ # noqa: E501
-    id: Optional[StrictStr] = Field(default=None, description="An identifier to disambiguate requests (echoed by the server).")
-    shape: Optional[List[MapMatchWaypoint]] = Field(default=None, description="REQUIRED if `encoded_polyline` is not present. Note that `break` type locations are only supported when `shape_match` is set to `map_match`.")
-    encoded_polyline: Optional[StrictStr] = Field(default=None, description="REQUIRED if `shape` is not present. An encoded polyline (https://developers.google.com/maps/documentation/utilities/polylinealgorithm). Note that the polyline must be encoded with 6 digits of precision rather than the usual 5.")
-    costing: MapMatchCostingModel
-    costing_options: Optional[CostingOptions] = None
-    shape_match: Optional[StrictStr] = Field(default=None, description="Three snapping modes provide some control over how the map matching occurs. `edge_walk` is fast, but requires extremely precise data that matches the route graph almost perfectly. `map_snap` can handle significantly noisier data, but is very expensive. `walk_or_snap`, the default, tries to use edge walking first and falls back to map matching if edge walking fails. In general, you should not need to change this parameter unless you want to trace a multi-leg route with multiple `break` locations in the `shape`.")
     units: Optional[DistanceUnit] = None
     language: Optional[ValhallaLanguages] = None
     directions_type: Optional[StrictStr] = Field(default='instructions', description="The level of directional narrative to include. Locations and times will always be returned, but narrative generation verbosity can be controlled with this parameter.")
-    filters: Optional[TraceAttributeFilterOptions] = Field(default=None, description="If present, provides either a whitelist or a blacklist of keys to include/exclude in the response. This key is optional, and if omitted from the request, all available info will be returned.")
+    id: Optional[StrictStr] = Field(default=None, description="An identifier to disambiguate requests (echoed by the server).")
+    locations: Annotated[List[RoutingWaypoint], Field(min_length=2)]
+    costing: CostingModel
+    costing_options: Optional[CostingOptions] = None
+    exclude_locations: Optional[List[RoutingWaypoint]] = Field(default=None, description="This has the same format as the locations list. Locations are mapped to the closed road(s), and these road(s) are excluded from the route path computation.")
+    exclude_polygons: Optional[List[List[List[Union[StrictFloat, StrictInt]]]]] = Field(default=None, description="One or multiple exterior rings of polygons in the form of nested JSON arrays. Roads intersecting these rings will be avoided during path finding. Open rings will be closed automatically. If you only need to avoid a few specific roads, it's much more efficient to use `exclude_locations`.")
+    alternates: Optional[StrictInt] = Field(default=None, description="How many alternate routes are desired. Note that fewer or no alternates may be returned. Alternates are not yet supported on routes with more than 2 locations or on time-dependent routes.")
+    elevation_interval: Optional[Union[StrictFloat, StrictInt]] = Field(default=0.0, description="If greater than zero, attempts to include elevation along the route at regular intervals. The \"native\" internal resolution is 30m, so we recommend you use this when possible. This number is interpreted as either meters or feet depending on the unit parameter. Elevation for route sections containing a bridge or tunnel is interpolated linearly. This doesn't always match the true elevation of the bridge/tunnel, but it prevents sharp artifacts from the surrounding terrain. This functionality is unique to the route endpoint and is not available via the elevation API.")
+    roundabout_exits: Optional[StrictBool] = Field(default=True, description="Determines whether the output should include roundabout exit instructions.")
     additional_properties: Dict[str, Any] = {}
-    __properties: ClassVar[List[str]] = ["id", "shape", "encoded_polyline", "costing", "costing_options", "shape_match", "units", "language", "directions_type", "filters"]
-
-    @field_validator('shape_match')
-    def shape_match_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['edge_walk', 'map_snap', 'walk_or_snap']):
-            raise ValueError("must be one of enum values ('edge_walk', 'map_snap', 'walk_or_snap')")
-        return value
+    __properties: ClassVar[List[str]] = ["units", "language", "directions_type", "id", "locations", "costing", "costing_options", "exclude_locations", "exclude_polygons", "alternates", "elevation_interval", "roundabout_exits"]
 
     @field_validator('directions_type')
     def directions_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -80,15 +72,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TraceAttributesRequest from a JSON string"""
+        """Create an instance of RouteRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -103,54 +95,60 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in shape (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in locations (list)
         _items = []
-        if self.shape:
-            for _item in self.shape:
+        if self.locations:
+            for _item in self.locations:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['shape'] = _items
+            _dict['locations'] = _items
         # override the default output from pydantic by calling `to_dict()` of costing_options
         if self.costing_options:
             _dict['costing_options'] = self.costing_options.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of filters
-        if self.filters:
-            _dict['filters'] = self.filters.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in exclude_locations (list)
+        _items = []
+        if self.exclude_locations:
+            for _item in self.exclude_locations:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['exclude_locations'] = _items
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TraceAttributesRequest from a dict"""
+        """Create an instance of RouteRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "shape": [MapMatchWaypoint.from_dict(_item) for _item in obj["shape"]] if obj.get("shape") is not None else None,
-            "encoded_polyline": obj.get("encoded_polyline"),
-            "costing": obj.get("costing"),
-            "costing_options": CostingOptions.from_dict(obj["costing_options"]) if obj.get("costing_options") is not None else None,
-            "shape_match": obj.get("shape_match"),
             "units": obj.get("units"),
             "language": obj.get("language"),
             "directions_type": obj.get("directions_type") if obj.get("directions_type") is not None else 'instructions',
-            "filters": TraceAttributeFilterOptions.from_dict(obj["filters"]) if obj.get("filters") is not None else None
+            "id": obj.get("id"),
+            "locations": [RoutingWaypoint.from_dict(_item) for _item in obj["locations"]] if obj.get("locations") is not None else None,
+            "costing": obj.get("costing"),
+            "costing_options": CostingOptions.from_dict(obj["costing_options"]) if obj.get("costing_options") is not None else None,
+            "exclude_locations": [RoutingWaypoint.from_dict(_item) for _item in obj["exclude_locations"]] if obj.get("exclude_locations") is not None else None,
+            "exclude_polygons": obj.get("exclude_polygons"),
+            "alternates": obj.get("alternates"),
+            "elevation_interval": obj.get("elevation_interval") if obj.get("elevation_interval") is not None else 0.0,
+            "roundabout_exits": obj.get("roundabout_exits") if obj.get("roundabout_exits") is not None else True
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
 
         return _obj
```

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of_filters.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attributes_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/trace_edge.py` & `stadiamaps-3.1.0/stadiamaps/models/trace_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/travel_mode.py` & `stadiamaps-3.1.0/stadiamaps/models/travel_mode.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/traversability.py` & `stadiamaps-3.1.0/stadiamaps/models/traversability.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/truck_costing_options.py` & `stadiamaps-3.1.0/stadiamaps/models/truck_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/truck_costing_options_all_of.py` & `stadiamaps-3.1.0/stadiamaps/models/truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/tz_response.py` & `stadiamaps-3.1.0/stadiamaps/models/tz_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/valhalla_languages.py` & `stadiamaps-3.1.0/stadiamaps/models/valhalla_languages.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/valhalla_long_units.py` & `stadiamaps-3.1.0/stadiamaps/models/valhalla_long_units.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/models/warning.py` & `stadiamaps-3.1.0/stadiamaps/models/warning.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/stadiamaps/rest.py` & `stadiamaps-3.1.0/stadiamaps/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,14 +199,16 @@
                         preload_content=False
                     )
                 elif content_type == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
+                    # Ensures that dict objects are serialized
+                    post_params = [(a, json.dumps(b)) if isinstance(b, dict) else (a,b) for a, b in post_params]
                     r = self.pool_manager.request(
                         method,
                         url,
                         fields=post_params,
                         encode_multipart=True,
                         timeout=timeout,
                         headers=headers,
```

### Comparing `stadiamaps-3.0.0/stadiamaps.egg-info/PKG-INFO` & `stadiamaps-3.1.0/stadiamaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 3.0.0
+Version: 3.1.0
 Summary: Stadia Maps Geospatial APIs
 Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-3.0.0/stadiamaps.egg-info/SOURCES.txt` & `stadiamaps-3.1.0/stadiamaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/integration/test_eu_endpoint.py` & `stadiamaps-3.1.0/test/integration/test_eu_endpoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/integration/test_gecoding.py` & `stadiamaps-3.1.0/test/integration/test_gecoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/integration/test_geospatial.py` & `stadiamaps-3.1.0/test/integration/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/integration/test_routing.py` & `stadiamaps-3.1.0/test/integration/test_routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,37 @@
             res = api_instance.route(req)
             self.assertEqual(req.id, res.id)
             self.assertEqual(0, res.trip.status)
             self.assertEqual("miles", res.trip.units)
             self.assertEqual(len(res.trip.legs), 1)
             self.assertEqual(len(res.alternates), 1)
 
+    def testRouteWithElevation(self):
+        with stadiamaps.ApiClient(self.configuration) as api_client:
+            api_instance = stadiamaps.RoutingApi(api_client)
+
+            req = stadiamaps.RouteRequest(
+                id="route",
+                locations=[
+                    stadiamaps.RoutingWaypoint.from_dict(location_a),
+                    stadiamaps.RoutingWaypoint.from_dict(location_b)
+                ],
+                costing=stadiamaps.CostingModel.AUTO,
+                costing_options=stadiamaps.CostingOptions(auto=stadiamaps.AutoCostingOptions(use_tolls=0.7)),
+                units=stadiamaps.DistanceUnit.MI,
+                elevation_interval=30,
+            )
+
+            res = api_instance.route(req)
+            self.assertEqual(req.id, res.id)
+            self.assertEqual(0, res.trip.status)
+            self.assertEqual("miles", res.trip.units)
+            self.assertEqual(len(res.trip.legs), 1)
+            self.assertGreater(len(res.trip.legs[0].elevation), 1)
+
     def testHybridBicycleRoute(self):
         # Regression test for user-reported issue
         with stadiamaps.ApiClient(self.configuration) as api_client:
             api_instance = stadiamaps.RoutingApi(api_client)
 
             req = stadiamaps.RouteRequest(
                 id="route",
```

### Comparing `stadiamaps-3.0.0/test/test_access.py` & `stadiamaps-3.1.0/test/test_access.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_admin_region.py` & `stadiamaps-3.1.0/test/test_admin_region.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_administrative.py` & `stadiamaps-3.1.0/test/test_administrative.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_auto_costing_options.py` & `stadiamaps-3.1.0/test/test_auto_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_auto_costing_options_all_of.py` & `stadiamaps-3.1.0/test/test_auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_base_costing_options.py` & `stadiamaps-3.1.0/test/test_base_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_base_trace_request.py` & `stadiamaps-3.1.0/test/test_base_trace_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_bicycle_costing_options.py` & `stadiamaps-3.1.0/test/test_bicycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_bicycle_costing_options_all_of.py` & `stadiamaps-3.1.0/test/test_bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_bike_network.py` & `stadiamaps-3.1.0/test/test_bike_network.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_contour.py` & `stadiamaps-3.1.0/test/test_contour.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_coordinate.py` & `stadiamaps-3.1.0/test/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_costing_model.py` & `stadiamaps-3.1.0/test/test_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_costing_options.py` & `stadiamaps-3.1.0/test/test_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_directions_options.py` & `stadiamaps-3.1.0/test/test_directions_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_distance_unit.py` & `stadiamaps-3.1.0/test/test_distance_unit.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_edge_sign.py` & `stadiamaps-3.1.0/test/test_edge_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_edge_use.py` & `stadiamaps-3.1.0/test/test_edge_use.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_end_node.py` & `stadiamaps-3.1.0/test/test_end_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_attributes.py` & `stadiamaps-3.1.0/test/test_geo_attributes.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_geometry.py` & `stadiamaps-3.1.0/test/test_geo_json_geometry.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_geometry_base.py` & `stadiamaps-3.1.0/test/test_geo_json_geometry_base.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_line_string.py` & `stadiamaps-3.1.0/test/test_geo_json_line_string.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_line_string_all_of.py` & `stadiamaps-3.1.0/test/test_geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_point.py` & `stadiamaps-3.1.0/test/test_geo_json_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_point_all_of.py` & `stadiamaps-3.1.0/test/test_geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_polygon.py` & `stadiamaps-3.1.0/test/test_geo_json_polygon.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geo_json_polygon_all_of.py` & `stadiamaps-3.1.0/test/test_geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geocoding_api.py` & `stadiamaps-3.1.0/test/test_geocoding_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geocoding_object.py` & `stadiamaps-3.1.0/test/test_geocoding_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_geospatial_api.py` & `stadiamaps-3.1.0/test/test_geospatial_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_height_request.py` & `stadiamaps-3.1.0/test/test_height_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_height_response.py` & `stadiamaps-3.1.0/test/test_height_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_highway_classification.py` & `stadiamaps-3.1.0/test/test_highway_classification.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_intersecting_edge.py` & `stadiamaps-3.1.0/test/test_intersecting_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_isochrone_costing_model.py` & `stadiamaps-3.1.0/test/test_isochrone_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_isochrone_feature.py` & `stadiamaps-3.1.0/test/test_isochrone_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_isochrone_properties.py` & `stadiamaps-3.1.0/test/test_isochrone_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_isochrone_request.py` & `stadiamaps-3.1.0/test/test_isochrone_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_isochrone_response.py` & `stadiamaps-3.1.0/test/test_isochrone_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_locate_detailed_edge.py` & `stadiamaps-3.1.0/test/test_locate_detailed_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_locate_edge.py` & `stadiamaps-3.1.0/test/test_locate_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_locate_edge_info.py` & `stadiamaps-3.1.0/test/test_locate_edge_info.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_locate_node.py` & `stadiamaps-3.1.0/test/test_locate_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_locate_node_all_of.py` & `stadiamaps-3.1.0/test/test_locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_locate_object.py` & `stadiamaps-3.1.0/test/test_locate_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_low_speed_vehicle_costing_options.py` & `stadiamaps-3.1.0/test/test_low_speed_vehicle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_maneuver_sign.py` & `stadiamaps-3.1.0/test/test_maneuver_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_maneuver_sign_element.py` & `stadiamaps-3.1.0/test/test_maneuver_sign_element.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_costing_model.py` & `stadiamaps-3.1.0/test/test_map_match_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_request.py` & `stadiamaps-3.1.0/test/test_map_match_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_request_all_of.py` & `stadiamaps-3.1.0/test/test_map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_route_response.py` & `stadiamaps-3.1.0/test/test_map_match_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_route_response_all_of.py` & `stadiamaps-3.1.0/test/test_map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_trace_options.py` & `stadiamaps-3.1.0/test/test_map_match_trace_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_waypoint.py` & `stadiamaps-3.1.0/test/test_map_match_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_map_match_waypoint_all_of.py` & `stadiamaps-3.1.0/test/test_map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_matched_point.py` & `stadiamaps-3.1.0/test/test_matched_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_matrix_costing_model.py` & `stadiamaps-3.1.0/test/test_matrix_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_matrix_distance.py` & `stadiamaps-3.1.0/test/test_matrix_distance.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_matrix_request.py` & `stadiamaps-3.1.0/test/test_matrix_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_matrix_response.py` & `stadiamaps-3.1.0/test/test_matrix_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_matrix_waypoint.py` & `stadiamaps-3.1.0/test/test_matrix_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_motor_scooter_costing_options.py` & `stadiamaps-3.1.0/test/test_motor_scooter_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_motor_scooter_costing_options_all_of.py` & `stadiamaps-3.1.0/test/test_motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_motorcycle_costing_options.py` & `stadiamaps-3.1.0/test/test_motorcycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_motorcycle_costing_options_all_of.py` & `stadiamaps-3.1.0/test/test_motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_nearest_roads_request.py` & `stadiamaps-3.1.0/test/test_nearest_roads_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_node_id.py` & `stadiamaps-3.1.0/test/test_node_id.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_node_type.py` & `stadiamaps-3.1.0/test/test_node_type.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_optimized_route_request.py` & `stadiamaps-3.1.0/test/test_optimized_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pedestrian_costing_options.py` & `stadiamaps-3.1.0/test/test_pedestrian_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_geo_json_feature.py` & `stadiamaps-3.1.0/test/test_pelias_geo_json_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_geo_json_properties.py` & `stadiamaps-3.1.0/test/test_pelias_geo_json_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum.py` & `stadiamaps-3.1.0/test/test_pelias_geo_json_properties_addendum.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-3.1.0/test/test_pelias_geo_json_properties_addendum_osm.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_layer.py` & `stadiamaps-3.1.0/test/test_pelias_layer.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_response.py` & `stadiamaps-3.1.0/test/test_pelias_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_response_geocoding.py` & `stadiamaps-3.1.0/test/test_pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_pelias_source.py` & `stadiamaps-3.1.0/test/test_pelias_source.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_restrictions.py` & `stadiamaps-3.1.0/test/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_road_class.py` & `stadiamaps-3.1.0/test/test_road_class.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_leg.py` & `stadiamaps-3.1.0/test/test_route_leg.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_maneuver.py` & `stadiamaps-3.1.0/test/test_route_maneuver.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_request.py` & `stadiamaps-3.1.0/test/test_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_response.py` & `stadiamaps-3.1.0/test/test_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_response_alternates_inner.py` & `stadiamaps-3.1.0/test/test_route_response_alternates_inner.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_response_trip.py` & `stadiamaps-3.1.0/test/test_route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_summary.py` & `stadiamaps-3.1.0/test/test_route_summary.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_route_trip.py` & `stadiamaps-3.1.0/test/test_route_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_routing_api.py` & `stadiamaps-3.1.0/test/test_routing_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_routing_response_waypoint.py` & `stadiamaps-3.1.0/test/test_routing_response_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_routing_response_waypoint_all_of.py` & `stadiamaps-3.1.0/test/test_routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_routing_waypoint.py` & `stadiamaps-3.1.0/test/test_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_routing_waypoint_all_of.py` & `stadiamaps-3.1.0/test/test_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_routing_waypoint_all_of_search_filter.py` & `stadiamaps-3.1.0/test/test_routing_waypoint_all_of_search_filter.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_simple_routing_waypoint.py` & `stadiamaps-3.1.0/test/test_simple_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_simple_routing_waypoint_all_of.py` & `stadiamaps-3.1.0/test/test_simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_speeds.py` & `stadiamaps-3.1.0/test/test_speeds.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attribute_filter_options.py` & `stadiamaps-3.1.0/test/test_trace_attribute_filter_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attribute_key.py` & `stadiamaps-3.1.0/test/test_trace_attribute_key.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attributes_base_response.py` & `stadiamaps-3.1.0/test/test_trace_attributes_base_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attributes_request.py` & `stadiamaps-3.1.0/test/test_trace_attributes_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attributes_request_all_of.py` & `stadiamaps-3.1.0/test/test_trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attributes_request_all_of_filters.py` & `stadiamaps-3.1.0/test/test_trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attributes_response.py` & `stadiamaps-3.1.0/test/test_trace_attributes_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_attributes_response_all_of.py` & `stadiamaps-3.1.0/test/test_trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_trace_edge.py` & `stadiamaps-3.1.0/test/test_trace_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_travel_mode.py` & `stadiamaps-3.1.0/test/test_travel_mode.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_traversability.py` & `stadiamaps-3.1.0/test/test_traversability.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_truck_costing_options.py` & `stadiamaps-3.1.0/test/test_truck_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_truck_costing_options_all_of.py` & `stadiamaps-3.1.0/test/test_truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_tz_response.py` & `stadiamaps-3.1.0/test/test_tz_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_valhalla_languages.py` & `stadiamaps-3.1.0/test/test_valhalla_languages.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_valhalla_long_units.py` & `stadiamaps-3.1.0/test/test_valhalla_long_units.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-3.0.0/test/test_warning.py` & `stadiamaps-3.1.0/test/test_warning.py`

 * *Files identical despite different names*

