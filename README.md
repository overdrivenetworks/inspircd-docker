# InspIRCd Docker Images for overdrive-irc

[![Build Status](https://drone.overdrivenetworks.com/api/badges/overdrivenetworks/inspircd-docker/status.svg)](https://drone.overdrivenetworks.com/overdrivenetworks/inspircd-docker)

This repository contains custom builds of InspIRCd for overdrive-irc. It is mostly the same as the [upstream image](https://github.com/inspircd/inspircd-docker), with some extra and contrib modules enabled by default.

As of 2020-02-23, these include:

## Core extras
- m_sslrehashsignal.cpp
- m_geo_maxmind.cpp

## Contrib modules
- m_blockhighlight
- m_xlinetools
- m_join0
- m_opmoderated
- m_fakelist

## Deployment Notes

This is not an official image so please don't treat it as such. I only support using a full custom config, i.e. mounting inspircd.conf under `/inspircd/conf/`.
