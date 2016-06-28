cmake_minimum_required(VERSION 3.5)
project (afcluster)
include_directories("${afcluster_SOURCE_DIR}")
set(SOURCES centroid.cc dists.cc em.cc freqs.cc hc.cc seqio.cc afcluster.cc centroid.hh dists.hh em.hh freqs.hh hc.hh seqio.hh
        )
file(GLOB SOURCES "*.cc")
file(GLOB SOURCES "*.hh")
include_directories(.)

add_executable(afscluster afcluster.cc centroid.cc dists.cc em.cc freqs.cc hc.cc seqio.cc)

