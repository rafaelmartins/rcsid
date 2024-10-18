# SPDX-FileCopyrightText: 2024 Rafael G. Martins <rafael@rafaelmartins.eng.br>
# SPDX-License-Identifier: GPL-2.0-or-later

add_library(resid INTERFACE)

target_sources(resid INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/envelope.cc
    ${CMAKE_CURRENT_LIST_DIR}/extfilt.cc
    ${CMAKE_CURRENT_LIST_DIR}/filter.cc
    ${CMAKE_CURRENT_LIST_DIR}/pot.cc
    ${CMAKE_CURRENT_LIST_DIR}/sid.cc
    ${CMAKE_CURRENT_LIST_DIR}/version.cc
    ${CMAKE_CURRENT_LIST_DIR}/voice.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave6581_PST.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave6581_PS_.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave6581_P_T.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave6581__ST.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave8580_PST.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave8580_PS_.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave8580_P_T.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave8580__ST.cc
)

target_include_directories(resid INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}
)

target_compile_definitions(resid INTERFACE
    VERSION="0.16"
)
