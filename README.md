# SPCast
### Modern Platform for Web Radio Streaming

SPCast was developed in a modular way. This page lists all dependencies.

It helps me keep an overview of all parts of the system.
The official project website is [https://www.spcast.eu](https://www.spcast.eu).
The repositories that are public are available to give interested users some insight into the platform.

It's a closed platform. We're using GitHub for some automation tasks.
Maybe one day we'll open the full codebase.

## SPCast.Frontend (Private)

This is the SPCast interface that allows users to manage their environment. Because the company uses WHMCS, the frontend is based on the Smarty Template Engine.

https://github.com/STREAMPANEL/SPCast.Frontend

## SPCast.Loadbalancer (Private)

This is the load balancer that manages all listeners across all stations.
(Contains sensitive data. Not public.)

## SPCast.News (Public)

This is the Liquidsoap component that sends news to stations if configured by the user.

https://github.com/STREAMPANEL/SPCast.News

## SPCast.Jingles (Public)

This is the Liquidsoap component that sends jingles to stations if configured by the user.

https://github.com/STREAMPANEL/SPCast.Jingles

## SPCast.Syndication (Public)

This is the Liquidsoap component that handles syndication to stations if configured by the user.

https://github.com/STREAMPANEL/SPCast.Syndication

## SPCast.PlayerDefault (Public)

This repository contains the default HTML5 player for all stations.

https://github.com/STREAMPANEL/SPCast.PlayerDefault

## SPCast.Recorder (Public)

This is the Liquidsoap component that records stations if configured by the user.

https://github.com/STREAMPANEL/SPCast.Recorder

## SPCast.SilenceDetection (Public)

This detects silence on stations and reacts accordingly.

https://github.com/STREAMPANEL/SPCast.SilenceDetection

## SPCast.Transcoder (Public)

This converts radio streams into multiple bitrates.
Currently supported: 256 Kbit/s MP3, 192 Kbit/s MP3, 128 Kbit/s MP3, 96 Kbit/s MP3, 64 Kbit/s AAC, 48 Kbit/s AAC, 32 Kbit/s AAC.

https://github.com/STREAMPANEL/SPCast.Transcoder

## SP--Cast---Skeleton (Private)

This contains the core environment, stream servers, and more. Without it, nothing works.
(Private due to a custom server codebase.)

## SPCast.FlutterManagement (Public)

Planned. Will be public once developed.

## SPCast.FlutterListeners (Public)

Planned. Will be public once developed.

## SPCast.Cron (Private)

Contains rules and scripts to prepare necessary files for all users.

## SPCast.Installer (Private)

Fully installs everything needed on fresh instances. We use Ubuntu LTS only. Currently: Ubuntu 22.04.

## SPCast.AutoDJ (Private)

Right now, we use [AzuraCast](https://github.com/AzuraCast/AzuraCast) as the AutoDJ. To run it without Docker, we use [this installer](https://github.com/scysys/AzuraCast-Ubuntu).
Originally, we planned to develop our own AutoDJ, which we still intend to do later in SPCast's development.
But time is short, and we want to move away from Centova Cast for several reasons. So for now, AzuraCast is a solid alternative.

## Other Dependencies

SPCast wouldn't work the way it does without the following:

- [Liquidsoap](https://github.com/savonet/liquidsoap)
- [Zabbix](https://github.com/zabbix/zabbix)
- [InfluxDB](https://github.com/influxdata/influxdb)
- [Grafana](https://github.com/grafana/grafana)
- [GoAccess](https://github.com/allinurl/goaccess)
- [FFmpeg](https://github.com/FFmpeg/FFmpeg)
- [AzuraCast](https://github.com/AzuraCast/AzuraCast)
- [AzuraCast - Traditional Installer](https://github.com/scysys/AzuraCast-Ubuntu)
