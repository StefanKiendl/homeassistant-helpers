# homeassistant-helpers

## Introduction

Smart home is fun and fancy, but also make living more comfortable and even more sustainable sometimes

But getting it configured and integrated properly, briding the various different technologies, protocols and busses is hard sometimes.
It took me hours or days sometimes to find things out, do the necessary research or even reverse engineer some interfaces, to get it properly integrated.

Some of the more difficult things around that, is what I want to share in this repo.


## Quick overview around my setup

I use [Home Assistant](https://www.home-assistant.io) running on a [ZimaBoard 832](https://www.zimaspace.com/products/single-board-server) as the central automation server
The backbone in my house are built on [KNX](https://www.knx.org/) and [Modbus](https://modbus.org/). KNX is running independent and providing all the MUST have base functionality.

For KNX I mainly use the awesome components from German manufacturer MDT, but also some other devices for some purposes.

Energy management system, heating controller and air ventilation are connected over Modbus TCP.
