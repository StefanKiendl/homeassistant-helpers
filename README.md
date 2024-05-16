# Solutions for Smart Home device/infrastructure integration using Home Assistant

## Introduction

Smart home is fun and fancy, makes living more comfortable and even more sustainable sometimes.

But getting everything integrated and configured properly, briding the various different technologies, protocols and busses is hard sometimes. Even for experts.
One of the biggest challenges is the 
It took me hours or days sometimes to find things out, do the necessary research or even reverse engineer some interfaces, to get it properly integrated.

Some of the more difficult things around that, is what I want to share in this repo.


## Quick overview around my setup

I use [Home Assistant](https://www.home-assistant.io) running on a [ZimaBoard 832](https://www.zimaspace.com/products/single-board-server) as central automation and integration server.

The backbone in my house is built on [KNX](https://www.knx.org/) and [Modbus](https://modbus.org/). KNX is running independent and providing all the MUST have base functionality
also to ensure "Non-Tech-People-Acceptance-Factor" is positive.

For KNX I mainly use the awesome components from German manufacturer [MDT](https://www.mdt.de/), but also some other devices for some purposes.

Energy management system, heating controller and air ventilation are connected over Modbus TCP.


## Open Issues

* Connect Solar heating controller to ethernet; special challenge is the properietary VBus interface with quite expensive adapters
* Water cleaning system has a REST interface with a quite weird interface design and response codes, that Home Assistant cannot process with the capabilities of the REST adapter out-of-the-box.
