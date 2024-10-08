# SPDX-FileCopyrightText: 2024 Rafael G. Martins <rafael@rafaelmartins.eng.br>
# SPDX-License-Identifier: GPL-2.0-or-later

add_library(resid INTERFACE)

target_sources(resid INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/dac.cc
    ${CMAKE_CURRENT_LIST_DIR}/envelope.cc
    ${CMAKE_CURRENT_LIST_DIR}/extfilt.cc
    ${CMAKE_CURRENT_LIST_DIR}/filter8850.cc
    ${CMAKE_CURRENT_LIST_DIR}/pot.cc
    ${CMAKE_CURRENT_LIST_DIR}/sid.cc
    ${CMAKE_CURRENT_LIST_DIR}/version.cc
    ${CMAKE_CURRENT_LIST_DIR}/voice.cc
    ${CMAKE_CURRENT_LIST_DIR}/wave.cc
)

target_include_directories(resid INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}
)
