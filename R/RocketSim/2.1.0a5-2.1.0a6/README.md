# Comparing `tmp/RocketSim-2.1.0a5.tar.gz` & `tmp/RocketSim-2.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RocketSim-2.1.0a5.tar", last modified: Sun May  5 03:03:48 2024, max compression
+gzip compressed data, was "RocketSim-2.1.0a6.tar", last modified: Sun May  5 18:57:46 2024, max compression
```

## Comparing `RocketSim-2.1.0a5.tar` & `RocketSim-2.1.0a6.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.052474 RocketSim-2.1.0a5/RocketSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 03:03:48.000000 RocketSim-2.1.0a5/RocketSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29474 2024-05-05 03:03:48.000000 RocketSim-2.1.0a5/RocketSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 03:03:48.000000 RocketSim-2.1.0a5/RocketSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 03:03:48.000000 RocketSim-2.1.0a5/RocketSim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 03:03:48.000000 RocketSim-2.1.0a5/RocketSim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.044474 RocketSim-2.1.0a5/libsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.052474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.044474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.052474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    37735 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    40585 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.060474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22714 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    48206 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h
--rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.064474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.068474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)    26341 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h
--rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.044474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.072474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h
--rw-r--r--   0 runner    (1001) docker     (127)    86089 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.072474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)    34628 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.072474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.076474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.080474 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h
--rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHull.h
--rw-r--r--   0 runner    (1001) docker     (127)    56111 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btHashMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btList.h
--rw-r--r--   0 runner    (1001) docker     (127)    43774 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMatrixX.h
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMinMax.h
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMotionState.h
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuadWord.h
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuickprof.h
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btReducedVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btScalar.h
--rw-r--r--   0 runner    (1001) docker     (127)   128666 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSerializer.h
--rw-r--r--   0 runner    (1001) docker     (127)   128676 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btThreads.h
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btTransform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    57838 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38269 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btVector3.h
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/btBulletCollisionCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/libsrc/bullet3-3.24/btBulletDynamicsCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.080474 RocketSim-2.1.0a5/python-mtheall/
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Angle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    94546 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Ball.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/BallHitInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/BallState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/BoostPad.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/BoostPadState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13598 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Car.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/CarConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/CarControls.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    35070 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/CarState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/DemoMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/GameMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/MemoryWeightMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Module.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    27079 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Module.h
--rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/MutatorConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/PyRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/RotMat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Team.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/Vec.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/WheelPairConfig.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     7834 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/regression_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73848 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/python-mtheall/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/BaseInc.h
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/BulletLink.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/BulletLink.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/CollisionMeshFile/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/CollisionMeshFile/CollisionMeshFile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/CollisionMeshFile/CollisionMeshFile.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/DataStream/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/DataStream/DataStreamIn.h
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/DataStream/DataStreamOut.h
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/DataStream/SerializeObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Framework.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Math/
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Math/Math.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Math/Math.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Math/MathTypes/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Math/MathTypes/MathTypes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Math/MathTypes/MathTypes.h
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/RLConst.h
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/RocketSim.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/RocketSim.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/Arena/
--rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Arena/Arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Arena/Arena.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/Ball/
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Ball/Ball.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Ball/Ball.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/BallHitInfo/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BallHitInfo/BallHitInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BallHitInfo/BallHitInfo.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/BallPredTracker/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BallPredTracker/BallPredTracker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BallPredTracker/BallPredTracker.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/BoostPad/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPad.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPad.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPadGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.084474 RocketSim-2.1.0a5/src/Sim/Car/
--rw-r--r--   0 runner    (1001) docker     (127)    28015 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Car/Car.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Car/Car.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/src/Sim/Car/CarConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Car/CarConfig/CarConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/Car/CarConfig/CarConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/CarControls.h
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/CollisionMasks.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/src/Sim/GameEventTracker/
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/GameEventTracker/GameEventTracker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/GameEventTracker/GameEventTracker.h
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/GameMode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/src/Sim/MutatorConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/MutatorConfig/MutatorConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/MutatorConfig/MutatorConfig.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/src/Sim/PhysState/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/PhysState/PhysState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/PhysState/PhysState.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/src/Sim/SuspensionCollisionGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 03:03:48.088474 RocketSim-2.1.0a5/src/Sim/btVehicleRL/
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/btVehicleRL/btVehicleRL.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-05 03:03:38.000000 RocketSim-2.1.0a5/src/Sim/btVehicleRL/btVehicleRL.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.307940 RocketSim-2.1.0a6/RocketSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29474 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 18:57:46.000000 RocketSim-2.1.0a6/RocketSim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.303940 RocketSim-2.1.0a6/libsrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.311940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.303940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.311940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37735 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40585 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.319940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22714 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48206 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.323940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.327940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26341 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.303940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.327940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    86089 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.331940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34628 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.331940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.335940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.335940 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56111 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btHashMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btList.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43774 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrixX.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMinMax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMotionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuadWord.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btScalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128666 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128676 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57838 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38269 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletCollisionCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletDynamicsCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.339940 RocketSim-2.1.0a6/python-mtheall/
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Angle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    94546 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Ball.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BallHitInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BallState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BoostPad.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/BoostPadState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13598 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Car.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/CarConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/CarControls.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/CarState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/DemoMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/GameMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/MemoryWeightMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Module.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/MutatorConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/PyRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/RotMat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Team.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/Vec.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/WheelPairConfig.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7834 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/regression_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73848 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/python-mtheall/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.339940 RocketSim-2.1.0a6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/BaseInc.h
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/BulletLink.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/BulletLink.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.339940 RocketSim-2.1.0a6/src/CollisionMeshFile/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/DataStream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/DataStream/DataStreamIn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/DataStream/DataStreamOut.h
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/DataStream/SerializeObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Framework.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Math/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/Math.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/Math.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Math/MathTypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/RLConst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/RocketSim.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/RocketSim.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Arena/
+-rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Arena/Arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Arena/Arena.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Ball/
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Ball/Ball.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Ball/Ball.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BallHitInfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallHitInfo/BallHitInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallHitInfo/BallHitInfo.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BallPredTracker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallPredTracker/BallPredTracker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BallPredTracker/BallPredTracker.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BoostPad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Car/
+-rw-r--r--   0 runner    (1001) docker     (127)    28015 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/Car.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/Car.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/Car/CarConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/CarControls.h
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/CollisionMasks.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/GameEventTracker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.h
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/GameMode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/MutatorConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/PhysState/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/PhysState/PhysState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/PhysState/PhysState.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.343940 RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:57:46.347940 RocketSim-2.1.0a6/src/Sim/btVehicleRL/
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-05 18:57:37.000000 RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.h
```

### Comparing `RocketSim-2.1.0a5/LICENSE` & `RocketSim-2.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/README.md` & `RocketSim-2.1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/RocketSim.egg-info/SOURCES.txt` & `RocketSim-2.1.0a6/RocketSim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LICENSE.txt` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHull.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btHashMap.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btHashMap.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btList.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btList.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMatrixX.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMatrixX.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMinMax.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMinMax.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btMotionState.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btMotionState.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuadWord.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuadWord.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuaternion.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuaternion.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btQuickprof.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btQuickprof.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btRandom.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btRandom.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btReducedVector.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btReducedVector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btScalar.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btScalar.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSerializer.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btThreads.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btThreads.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btThreads.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btTransform.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransform.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btVector3.cpp` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/LinearMath/btVector3.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/LinearMath/btVector3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/MANIFEST.in` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/README.md` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/README.md`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/btBulletCollisionCommon.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletCollisionCommon.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/libsrc/bullet3-3.24/btBulletDynamicsCommon.h` & `RocketSim-2.1.0a6/libsrc/bullet3-3.24/btBulletDynamicsCommon.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Angle.cpp` & `RocketSim-2.1.0a6/python-mtheall/Angle.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Arena.cpp` & `RocketSim-2.1.0a6/python-mtheall/Arena.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Array.cpp` & `RocketSim-2.1.0a6/python-mtheall/Array.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Array.h` & `RocketSim-2.1.0a6/python-mtheall/Array.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Ball.cpp` & `RocketSim-2.1.0a6/python-mtheall/Ball.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/BallHitInfo.cpp` & `RocketSim-2.1.0a6/python-mtheall/BallHitInfo.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/BallState.cpp` & `RocketSim-2.1.0a6/python-mtheall/BallState.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/BoostPad.cpp` & `RocketSim-2.1.0a6/python-mtheall/BoostPad.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/BoostPadState.cpp` & `RocketSim-2.1.0a6/python-mtheall/BoostPadState.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Car.cpp` & `RocketSim-2.1.0a6/python-mtheall/Car.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/CarConfig.cpp` & `RocketSim-2.1.0a6/python-mtheall/CarConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/CarControls.cpp` & `RocketSim-2.1.0a6/python-mtheall/CarControls.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/CarState.cpp` & `RocketSim-2.1.0a6/python-mtheall/CarState.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 #include "Module.h"
 
 #include <algorithm>
 #include <cstddef>
 #include <cstring>
+#include <mutex>
 
 namespace RocketSim::Python
 {
 constexpr unsigned NUM_WHEELS = std::extent_v<decltype (RocketSim::CarState::wheelsWithContact)>;
 
+std::once_flag lastRelDodgeTorqueWarnOnce;
+
+void warnLastRelDodgeTorque ()
+{
+	std::call_once (lastRelDodgeTorqueWarnOnce,
+	    &std::fprintf,
+	    stderr,
+	    "last_rel_dodge_torque is a deprecated alias of flip_rel_torque\n");
+}
+
 PyTypeObject *CarState::Type = nullptr;
 
 PyMemberDef CarState::Members[] = {
     {.name      = "update_counter",
         .type   = TypeHelper<decltype (RocketSim::CarState::updateCounter)>::type,
         .offset = offsetof (CarState, state) + offsetof (RocketSim::CarState, updateCounter),
         .flags  = 0,
@@ -163,14 +174,15 @@
 };
 
 PyGetSetDef CarState::GetSet[] = {
     GETSET_ENTRY (CarState, pos, "Position"),
     GETSET_ENTRY (CarState, rot_mat, "Rotation matrix"),
     GETSET_ENTRY (CarState, vel, "Velocity"),
     GETSET_ENTRY (CarState, ang_vel, "Angular velocity"),
+    GETSET_ENTRY (CarState, last_rel_dodge_torque, "Deprecated alias of flip_rel_torque"),
     GETSET_ENTRY (CarState, flip_rel_torque, "Flip relative torque"),
     GETSET_ENTRY (CarState, last_controls, "Last controls"),
     GETSET_ENTRY (CarState, world_contact_normal, "World contact normal"),
     GETSET_ENTRY (CarState, ball_hit_info, "Ball hit info"),
     GETSET_ENTRY (CarState, wheels_with_contact, "Wheels with contact"),
     {.name = nullptr, .get = nullptr, .set = nullptr, .doc = nullptr, .closure = nullptr},
 };
@@ -332,14 +344,15 @@
 	static char carContactIDKwd[]            = "car_contact_id";
 	static char carContactCooldownTimerKwd[] = "car_contact_cooldown_timer";
 	static char isDemoedKwd[]                = "is_demoed";
 	static char demoRespawnTimerKwd[]        = "demo_respawn_timer";
 	static char ballHitInfoKwd[]             = "ball_hit_info";
 	static char lastControlsKwd[]            = "last_controls";
 	static char updateCounterKwd[]           = "update_counter";
+	static char lastRelDodgeTorqueKwd[]      = "last_rel_dodge_torque";
 
 	static char *dict[] = {posKwd,
 	    rotMatKwd,
 	    velKwd,
 	    angVelKwd,
 	    isOnGroundKwd,
 	    wheelsWithContactKwd,
@@ -365,27 +378,29 @@
 	    carContactIDKwd,
 	    carContactCooldownTimerKwd,
 	    isDemoedKwd,
 	    demoRespawnTimerKwd,
 	    ballHitInfoKwd,
 	    lastControlsKwd,
 	    updateCounterKwd,
+	    lastRelDodgeTorqueKwd,
 	    nullptr};
 
 	RocketSim::CarState state{};
 
 	PyObject *pos                = nullptr; // borrowed references
 	PyObject *rotMat             = nullptr;
 	PyObject *vel                = nullptr;
 	PyObject *angVel             = nullptr;
 	PyObject *wheelsWithContact  = nullptr;
 	PyObject *flipRelTorque      = nullptr;
 	PyObject *lastControls       = nullptr;
 	PyObject *worldContactNormal = nullptr;
 	PyObject *ballHitInfo        = nullptr;
+	PyObject *lastRelDodgeTorque = nullptr;
 
 	int isOnGround      = state.isOnGround;
 	int hasJumped       = state.hasJumped;
 	int hasDoubleJumped = state.hasDoubleJumped;
 	int hasFlipped      = state.hasFlipped;
 	int isFlipping      = state.isFlipping;
 	int isJumping       = state.isJumping;
@@ -394,15 +409,15 @@
 	int hasWorldContact = state.worldContact.hasContact;
 	int isDemoed        = state.isDemoed;
 
 	unsigned long carContactID       = state.carContact.otherCarID;
 	unsigned long long updateCounter = state.updateCounter;
 	if (!PyArg_ParseTupleAndKeywords (args_,
 	        kwds_,
-	        "|O!O!O!O!pOpppO!ffppffffpffpfpO!kfpfO!O!K",
+	        "|O!O!O!O!pOpppO!ffppffffpffpfpO!kfpfO!O!K$O!",
 	        dict,
 	        Vec::Type,
 	        &pos,
 	        RotMat::Type,
 	        &rotMat,
 	        Vec::Type,
 	        &vel,
@@ -435,15 +450,17 @@
 	        &state.carContact.cooldownTimer,
 	        &isDemoed,
 	        &state.demoRespawnTimer,
 	        BallHitInfo::Type,
 	        &ballHitInfo,
 	        CarControls::Type,
 	        &lastControls,
-	        &updateCounter))
+	        &updateCounter,
+	        Vec::Type,
+	        &lastRelDodgeTorque))
 		return -1;
 
 	if (pos)
 		state.pos = Vec::ToVec (PyCast<Vec> (pos));
 
 	if (rotMat)
 		state.rotMat = RotMat::ToRotMat (PyCast<RotMat> (rotMat));
@@ -461,14 +478,16 @@
 			return -1;
 
 		std::copy (std::begin (tmp), std::end (tmp), std::begin (state.wheelsWithContact));
 	}
 
 	if (flipRelTorque)
 		state.flipRelTorque = Vec::ToVec (PyCast<Vec> (flipRelTorque));
+	else if (lastRelDodgeTorque)
+		state.flipRelTorque = Vec::ToVec (PyCast<Vec> (lastRelDodgeTorque));
 
 	if (worldContactNormal)
 		state.worldContact.contactNormal = Vec::ToVec (PyCast<Vec> (worldContactNormal));
 
 	if (ballHitInfo)
 		state.ballHitInfo = BallHitInfo::ToBallHitInfo (PyCast<BallHitInfo> (ballHitInfo));
 
@@ -844,14 +863,26 @@
 	}
 
 	PyRef<Vec>::assign (self_->angVel, value_);
 
 	return 0;
 }
 
+PyObject *CarState::Getlast_rel_dodge_torque (CarState *self_, void *closure_) noexcept
+{
+	warnLastRelDodgeTorque ();
+	return Getflip_rel_torque (self_, closure_);
+}
+
+int CarState::Setlast_rel_dodge_torque (CarState *self_, PyObject *value_, void *closure_) noexcept
+{
+	warnLastRelDodgeTorque ();
+	return Setflip_rel_torque (self_, value_, closure_);
+}
+
 PyObject *CarState::Getflip_rel_torque (CarState *self_, void *) noexcept
 {
 	return PyRef<Vec>::incRef (self_->flipRelTorque).giftObject ();
 }
 
 int CarState::Setflip_rel_torque (CarState *self_, PyObject *value_, void *) noexcept
 {
```

### Comparing `RocketSim-2.1.0a5/python-mtheall/Module.cpp` & `RocketSim-2.1.0a6/python-mtheall/Module.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Module.h` & `RocketSim-2.1.0a6/python-mtheall/Module.h`

 * *Files 0% similar despite different names*

```diff
@@ -561,14 +561,15 @@
 	static PyObject *HasFlipReset (CarState *self_) noexcept;
 	static PyObject *GotFlipReset (CarState *self_) noexcept;
 
 	GETSET_DECLARE (CarState, pos)
 	GETSET_DECLARE (CarState, rot_mat)
 	GETSET_DECLARE (CarState, vel)
 	GETSET_DECLARE (CarState, ang_vel)
+	GETSET_DECLARE (CarState, last_rel_dodge_torque)
 	GETSET_DECLARE (CarState, flip_rel_torque)
 	GETSET_DECLARE (CarState, last_controls)
 	GETSET_DECLARE (CarState, world_contact_normal)
 	GETSET_DECLARE (CarState, ball_hit_info)
 	GETSET_DECLARE (CarState, wheels_with_contact)
 };
```

### Comparing `RocketSim-2.1.0a5/python-mtheall/MutatorConfig.cpp` & `RocketSim-2.1.0a6/python-mtheall/MutatorConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/PyRef.h` & `RocketSim-2.1.0a6/python-mtheall/PyRef.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/RotMat.cpp` & `RocketSim-2.1.0a6/python-mtheall/RotMat.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/Vec.cpp` & `RocketSim-2.1.0a6/python-mtheall/Vec.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/WheelPairConfig.cpp` & `RocketSim-2.1.0a6/python-mtheall/WheelPairConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/regression_test.py` & `RocketSim-2.1.0a6/python-mtheall/regression_test.py`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/python-mtheall/unit_test.py` & `RocketSim-2.1.0a6/python-mtheall/unit_test.py`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/setup.py` & `RocketSim-2.1.0a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,13 +84,13 @@
     ("NO_IMPORT_ARRAY", "1"),
     ("RS_DONT_LOG", "1")
   ]
 )
 
 setup(
   name = "RocketSim",
-  version = "2.1.0a5",
+  version = "2.1.0a6",
   description = "This is Rocket League!",
   cmdclass = {"build_ext": build_ext_ex},
   ext_modules = [RocketSim],
   install_requires = ["numpy"]
 )
```

### Comparing `RocketSim-2.1.0a5/src/BulletLink.h` & `RocketSim-2.1.0a6/src/BulletLink.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/CollisionMeshFile/CollisionMeshFile.cpp` & `RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/CollisionMeshFile/CollisionMeshFile.h` & `RocketSim-2.1.0a6/src/CollisionMeshFile/CollisionMeshFile.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/DataStream/DataStreamIn.h` & `RocketSim-2.1.0a6/src/DataStream/DataStreamIn.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/DataStream/DataStreamOut.h` & `RocketSim-2.1.0a6/src/DataStream/DataStreamOut.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Framework.h` & `RocketSim-2.1.0a6/src/Framework.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Math/Math.cpp` & `RocketSim-2.1.0a6/src/Math/Math.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Math/Math.h` & `RocketSim-2.1.0a6/src/Math/Math.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Math/MathTypes/MathTypes.cpp` & `RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Math/MathTypes/MathTypes.h` & `RocketSim-2.1.0a6/src/Math/MathTypes/MathTypes.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/RLConst.h` & `RocketSim-2.1.0a6/src/RLConst.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/RocketSim.cpp` & `RocketSim-2.1.0a6/src/RocketSim.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/RocketSim.h` & `RocketSim-2.1.0a6/src/RocketSim.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Arena/Arena.cpp` & `RocketSim-2.1.0a6/src/Sim/Arena/Arena.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Arena/Arena.h` & `RocketSim-2.1.0a6/src/Sim/Arena/Arena.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Ball/Ball.cpp` & `RocketSim-2.1.0a6/src/Sim/Ball/Ball.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Ball/Ball.h` & `RocketSim-2.1.0a6/src/Sim/Ball/Ball.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BallHitInfo/BallHitInfo.h` & `RocketSim-2.1.0a6/src/Sim/BallHitInfo/BallHitInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BallPredTracker/BallPredTracker.cpp` & `RocketSim-2.1.0a6/src/Sim/BallPredTracker/BallPredTracker.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BallPredTracker/BallPredTracker.h` & `RocketSim-2.1.0a6/src/Sim/BallPredTracker/BallPredTracker.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPad.cpp` & `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPad.h` & `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPad.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp` & `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h` & `RocketSim-2.1.0a6/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Car/Car.cpp` & `RocketSim-2.1.0a6/src/Sim/Car/Car.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Car/Car.h` & `RocketSim-2.1.0a6/src/Sim/Car/Car.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Car/CarConfig/CarConfig.cpp` & `RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/Car/CarConfig/CarConfig.h` & `RocketSim-2.1.0a6/src/Sim/Car/CarConfig/CarConfig.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/CarControls.h` & `RocketSim-2.1.0a6/src/Sim/CarControls.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/GameEventTracker/GameEventTracker.cpp` & `RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/GameEventTracker/GameEventTracker.h` & `RocketSim-2.1.0a6/src/Sim/GameEventTracker/GameEventTracker.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/MutatorConfig/MutatorConfig.cpp` & `RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/MutatorConfig/MutatorConfig.h` & `RocketSim-2.1.0a6/src/Sim/MutatorConfig/MutatorConfig.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp` & `RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h` & `RocketSim-2.1.0a6/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/btVehicleRL/btVehicleRL.cpp` & `RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a5/src/Sim/btVehicleRL/btVehicleRL.h` & `RocketSim-2.1.0a6/src/Sim/btVehicleRL/btVehicleRL.h`

 * *Files identical despite different names*

