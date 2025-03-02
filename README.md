# Phantom + Meshtastic = Phantastic


## Overview

Meshtastic has been getting a lot of interest lately, especially among privacy focused groups for off-grid comms. While it uses encryption by default to keep private chats private, anonymization is not one key goals. This could lead to nodes being used to track individuals without their consent. There are situations where someone might want to use meshtastic node for communication with an ephemeral identity that can be later scrubbed, like at a protest or hacker convention. 

Enter Phantastic, a fork of meshtastic that aims to make profiling harder by completely regenerating all identifying information on a firmware reset, and make other tracking harder during normal usage. So a user can change their ID whenever it makes sense for them.

## What are the changes
- [x] Generate a random NodeID on firmware reset 
- [ ] Add Mac address randomization to ble 
- [ ] Add Mac address randomization to wifi
- [ ] Add random delay before sending message to avoid visual profiling of a user
- [ ] Add build job to release .bin files so users can flash with web flasher
- [ ] Other ideas? Submit them as an issue or PR!

## How can we trust you
You shouldn't trust me. Look at the code changes and judge for yourself. They are relatively simple. If possible, compile and flash from source instead of trusting a random .bin file uploaded by some random cyberpunk.


### Get Started

Follow the normal Meshtastic building and flashing instructions, just with this repo instead of the official one

- 🔧 **[Building Instructions](https://meshtastic.org/docs/development/firmware/build)** – Learn how to compile the firmware from source.
- ⚡ **[Flashing Instructions](https://meshtastic.org/docs/getting-started/flashing-firmware/)** – Install or update the firmware on your device.


