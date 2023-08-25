# ESMS

add_executable(esms)

target_compile_options(
  esms
  PRIVATE
    "-Wall" "-pedantic" "-Wextra"
)

target_sources(
  esms
  PRIVATE
    rosterplayer.cpp
    comment.cpp
    penalty.cpp
    report_event.cpp
    esms.cpp
    cond_utils.cpp
    teamsheet_reader.cpp
    cond_action.cpp
    cond_condition.cpp
    util.cpp
    cond.cpp
    mt.cpp
    config.cpp
    tactics.cpp
    anyoption.cpp
)

target_include_directories(
  esms
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_compile_features(
  esms
  PRIVATE
    cxx_std_20
)

# ROSTER_CREATOR

add_executable(roster_creator)

target_sources(
  roster_creator
  PRIVATE
    roster_creator.cpp
    rosterplayer.cpp
    anyoption.cpp
    config.cpp
    util.cpp
)

target_compile_options(
  roster_creator
  PRIVATE
    "-Wall" "-pedantic" "-Wextra"
)

target_include_directories(
  roster_creator
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_compile_features(
  roster_creator
  PRIVATE
    cxx_std_20
)

# LGTABLE

add_executable(lgtable)

target_sources(
  lgtable
  PRIVATE
    lgtable.cpp
    league_table.cpp
    util.cpp
    anyoption.cpp
)

target_compile_options(
  lgtable
  PRIVATE
    "-Wall" "-pedantic" "-Wextra"
)

target_include_directories(
  lgtable
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_compile_features(
  lgtable
  PRIVATE
    cxx_std_20
)

# UPDTR

add_executable(updtr)

target_sources(
  updtr
  PRIVATE
    rosterplayer.cpp
    updtr.cpp
    util.cpp
    anyoption.cpp
    config.cpp
    comment.cpp
    league_table.cpp
)

target_compile_options(
  updtr
  PRIVATE
    "-Wall" "-pedantic" "-Wextra"
)

target_include_directories(
  updtr
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_compile_features(
  updtr
  PRIVATE
    cxx_std_20
)

# FIXTURES

add_executable(fixtures)

target_sources(
  fixtures
  PRIVATE
    fixtures.cpp
    util.cpp
    anyoption.cpp
)

target_compile_options(
  fixtures
  PRIVATE
    "-Wall" "-pedantic" "-Wextra"
)

target_include_directories(
  fixtures
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_compile_features(
  fixtures
  PRIVATE
    cxx_std_20
)

# TSC

add_executable(tsc)

target_sources(
  tsc
  PRIVATE
    tsc.cpp
    rosterplayer.cpp
    util.cpp
    config.cpp
)

target_compile_options(
  tsc
  PRIVATE
    "-Wall" "-pedantic" "-Wextra"
)

target_include_directories(
  tsc
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

target_compile_features(
  tsc
  PRIVATE
    cxx_std_20
)