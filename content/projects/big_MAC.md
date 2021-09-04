---
title: "BigMAC: MACs of Interest Tracking"
date: 2020-12-04T16:05:13+01:00
Description: ""
Tags: []
Categories: []
DisableComments: false
---

## Objective:
Using a collection of ESP8266/NodeMCUs, build a network capable of tracking MACs of interest.

## Method:
WiFi devices send probing frames to check for faster connections. ESP8266 can pretend to be a validate network, to get these probing frames, enabling collection of the MAC address of WiFi devices. In combination with the RSSI values of the WiFi connection, we can approximate location based on signal strength.

In this project I also incorporated a GPS module to the ESP8266, which allows for the board to be spatially dynamic e.g. On a police car. The GPS provides a precise location of the board and the RSSI can provide a rough insight into proximity from the board.

To ensure ethical/legal integrity the network only searches for authorised "MACs of interest", hence does not record all MACs. Only authorized MACs have any data stored i.e. My own MACs for this project.

As a bonus, I also setup weather station ESP8266s, to data fuse with MAC movements.

## Uses:
Finding missing people, criminals, track politication movements for transparency...etc


## System Overview:

{{< figure src="/images/MACs_of_interest.png" >}}

## Frontend Overview:

{{< figure src="/images/MACs_of_interest_frontend.png" >}}

## Repo?

Making this repo public feels like a bad idea.