# OMCI Wireshark Dissector

## Introduction

Wireshark dissector for ONT Management and Control Interface (OMCI) protocol (ITU Rec. G984.4)

This protocol is used on Gigabit Passive Optical Network (GPON) between Optical Line Termition (OLT) and Optical Network Termination (ONT) units.

This is management protocol used to configure services (like Ethernet, Video overlay, Tx/RX control) on the ONT.

## Pre-requirements

The dissector is working with **Wirshark version 1.4.3** (or newer version). The Lua version should be at least **Lua 5.1**.

To see the version you have to go to menu [Help/About](https://github.com/0liv1er/omci-wireshark-dissector/raw/master/wirehark-about.png)

## Changed to be done in Wireshark configuration

* Go to your Wireshark project directory, on Windoze C:\Program Files\Wireshark
* Open file init.lua
* Add the following line at the end of this init.lua file: dofile("C:\\Path\\to\\my\\favourite\\folder\\omci.lua")
* Download source files from [GitHub](https://github.com/0liv1er/omci-wireshark-dissector)
* Copy both BinDecHex.lua and omci.lua files into Wireshark project directory

You're now ready.

You can test the dissector by using this [example](https://github.com/0liv1er/omci-wireshark-dissector/blob/master/omci-example.pcap?raw=true)
