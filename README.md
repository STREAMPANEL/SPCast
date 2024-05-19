# SPCast
### Modern Platform for Web Radio Streaming

SPCast was developed in a modular way. This page contains all dependencies.

This will help me not to lose the overview of all dependencies.
The Repositories that are open are here to give interested users an insight into the platform.

It's a closed platform. We're using GitHub for some automations.
Maybe one day we will open the full codebase.

## SPCast.Frontend (Private)

This is the SPCast interface through which users manage their environment accordingly. Due to the use of WHMCS in the company, the frontend has been implemented based on the Smarty Template Engine.

https://github.com/STREAMPANEL/SPCast.Frontend

## SPCast.Loadbalancer (Private)

This is the load balancer which takes care of all listeners over all stations.
(Contains sensitive information. Not public!)

## SPCast.News (Public)

This will be the Liquidsoap part which sends the news to stations if set up by the user.

https://github.com/STREAMPANEL/SPCast.News

## SPCast.Jingles (Public)

This will be the Liquidsoap part which sends the jingles to stations if set up by the user.

https://github.com/STREAMPANEL/SPCast.Jingles

## SPCast.Syndication (Public)

This will be the Liquidsoap part which sends the jingles to stations if set up by the user.

https://github.com/STREAMPANEL/SPCast.Syndication

## SPCast.PlayerDefault (Public)

This repository will contain the default HTML5 player for all stations.

https://github.com/STREAMPANEL/SPCast.PlayerDefault

## SPCast.Recorder (Public)

This will be the Liquidsoap part which records the stations if set up by the user.

https://github.com/STREAMPANEL/SPCast.Recorder

## SPCast.SilenceDetection (Public)

This will detect stations for silence and react to it.

https://github.com/STREAMPANEL/SPCast.SilenceDetection

## SPCast.Transcoder (Public)

This will convert users radio stations to all needed bitrates.
Currently, these are: 256 Kbit/s MP3, 192 Kbit/s MP3, 128 Kbit/s MP3, 96 Kbit/s MP3, 64 Kbit/s AAC, 48 Kbit/s AAC, 32 Kbit/s AAC.

https://github.com/STREAMPANEL/SPCast.Transcoder

## SP--Cast---Skeleton (Private)

This contains the main environment, streamservers, and so on. Without this, nothing will work.
(Private, because of custom server codebase.)

## SPCast.FlutterManagement (Public)

To be developed. (Will be public)

## SPCast.FlutterListeners (Public)

To be developed. (Will be public)

## SPCast.Cron (Private)

This repository contains rules and scripts that will prepare the files for all users that are needed.

## SPCast.Installer (Private)

This will install everything that is needed fully automatically on fresh instances. We're only using Ubuntu LTS releases. At this time, it is Ubuntu 22.04.

## SPCast.AutoDJ (Private)

Currently, we're using [AzuraCast](https://github.com/AzuraCast/AzuraCast) as AutoDJ. To make it work without Docker, we're using [this](https://github.com/scysys/AzuraCast-Ubuntu) repository.
Initially, we planned to also develop the AutoDJ on our own. We will do it at a later time of the SPCast platform.
But time is running out, and we want to move away from Centova Cast for a few reasons. So, for now, it's a great alternative.

## Other Dependencies

Without these other dependencies, SPCast will not be possible the way we've done it.

- [Liquidsoap](https://github.com/savonet/liquidsoap)
- [Zabbix](https://github.com/zabbix/zabbix)
- [Grafana](https://github.com/grafana/grafana)
- [GoAccess](https://github.com/allinurl/goaccess)
- [FFmpeg](https://github.com/FFmpeg/FFmpeg)
- [AzuraCast](https://github.com/AzuraCast/AzuraCast)
- [AzuraCast - Traditional Installer](https://github.com/scysys/AzuraCast-Ubuntu)
