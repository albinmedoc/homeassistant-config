<h1 align="center">
  🏠<br/>Home Assistant configuration for a smart-looking place!<br/> <sup><sub>by <a href="https://albinmedoc.se/">Albin Médoc</a> 😃</sub></sup>
</h1>
<p align="center"><strong>Be sure to ⭐️ my repo if you find it useful! 😃</strong></p>

> **Note:** This README is highly inspired by [renemarc](https://github.com/renemarc/home-assistant-config)'s.

## Table of contents 📑

1. **[TL;DR](#tldr-)**
2. **[Overview](#overview-)**\
    [Goals](#goals-) | [Agile development](#agile-development-)
3. **[Home Assistant add-ons](#home-assistant-add-ons-)**
4. **[Community Integrations](#community-integrations-%EF%B8%8F)**
5. **[License](#license-)**
6. **[Thanks](#thanks-)**

## TL;DR 🏃

This is a fully documented working configuration for Home Assistant, with screenshots, hints and comments. [Browse the code](https://github.com/albinmedoc/homeassistant-config/tree/master) to have a look! 👀

## Overview 🌅

### Goals ⚽

- **Inconspicuous**: I love tech alright, but like any good butlers it should stay out of sight yet stay summonable. Think Fiji villa, not server room.
- **Modular**: Both code and devices should be easily replaceable.
- **Internet independent**: As much local processing as possible for the essential features.
- **Accessible through multiple ways:** Computers, tablet (kiosk), voice, smart phones, wireless buttons, remotes.
- **Intuitive user interfaces:** One look at a group of sensors/switches should be sufficient for anyone to understand the current states and how to operate an interface. 💡
- **Redundant controls:** Multiple interfaces should be able to control devices without interference. State changes from manual interventions or dedicated manufacturer apps should be tracked whenever possible.
- **No information overload:** Provide just enough insights to get an idea of what's going on. And no need for data that's best consumed on more interactive devices (like stock prices, Steam community status…)

### Agile development 🖖

This configuration is built with an [Agile](http://agilemanifesto.org/)-like methodology, lead by following main user stories:

- **As a resident** I want a reliable home automation platform to handle lights and climate that can easily be controlled and overridden in many intuitive ways.
- **As a developer** I want to use an open-source platform that is feature-rich, accessible, flexible and actively maintained.
- **As a consumer** I want to pick and choose which devices I wish to acquire without necessarily being locked into a closed ecosystem.
- **As a couple** we want to be able to operate lights and climate-control appliances as well as get quick overview of weather forecasts and public transit schedules through simple to use interfaces.

Tasks are hopefully defined in the [issue queue][link-issues] and their development progress is managed using a [lightweight Kanban board][link-board].

<div align="center">
    <figure>
        <img src="https://i.imgur.com/jKGbzWV.jpg" alt="Agile. You keep using that word. I do not think it means what you think it means." width="480">
        <figcaption>
            <p><strong>Well, without the sprints. And a team. And the retrospectives. And the…</strong></p>
        </figcaption>
    </figure>
</div>

#### Home Assistant add-ons ➕

| `Add-on` | `Usage` |
|---------:|:--------|
| **[AdGuard Home](https://github.com/hassio-addons/addon-adguard-home)** | to remove ads from my whole network.
| **[Cloudflared](https://github.com/brenner-tobias/addon-cloudflared/)** | to use my own domain name and access HA outside my network.
| **[ESPHome](https://github.com/esphome/esphome)** | to create diy devices.
| **[Frigate](https://github.com/blakeblackshear/frigate)** | to identify motion and objects in camera feeds, used as DVR.
| **[Grafana](https://github.com/hassio-addons/addon-grafana)** | to create cool graphs and visualize long-term statistics.
| **[InfluxDB](https://github.com/hassio-addons/addon-influxdb)** | for long-term statistics.
| **[Maria DB](https://github.com/home-assistant/addons/tree/master/mariadb)** | databse used to store history and logbook.
| **[Mosquitto broker](https://github.com/home-assistant/addons/tree/master/mosquitto)** | to be able to add MQTT devices to HA.
| **[Node-RED](https://github.com/hassio-addons/addon-node-red)** | to create advanced and visual pleasing automations.
| **[Samba share](https://github.com/home-assistant/addons/tree/master/samba)** | to access my HA config through SMBD.
| **[SSH & Web Terminal](https://github.com/hassio-addons/addon-ssh)** | to be able to SSH into my HA server, useful if something goes realy bad.
| **[Studio Code Server](https://github.com/hassio-addons/addon-vscode)** | to easily edit my HA files.

#### Community integrations 🏘️

| `Integration` | `Usage` |
|--------------:|:--------|
| **[SamsungTV Tizen](https://github.com/jaruba/ha-samsungtv-tizen)** | to controll my samsung tv through HA.
| **[Tapo: Cameras Control](https://github.com/JurajNyiri/HomeAssistant-Tapo-Control)** | to add all my Tapo cameras into HA, supports ONVIF.
| **[browser_mod](https://github.com/thomasloven/hass-browser_mod)** | to add pop-up support in dashboard.
| **[Google WiFi](https://github.com/djtimca/hagooglewifi)** | to track devices at home, and number of devices connected to guest network.
| **[Alarmo](https://github.com/nielsfaber/alarmo)** | to easily create an alarm system.
| **[Remote Home Assistant](https://github.com/custom-components/remote_homeassistant)** | to expose entities to my parents Home Assistant.
| **[Frigate](https://github.com/blakeblackshear/frigate-hass-integration)** | to integrate Frigate into HA.
| **[Office 365 Integration](https://github.com/RogerSelwyn/O365-HomeAssistant)** | to integrate my work calendar.
| **[UI Lovelace Minimalist](https://github.com/UI-Lovelace-Minimalist/UI)** | used to create my dashboard.
| **[Swedish Mail Delivery](https://github.com/DSorlov/swemail)** | adds sensors to indicate when the mail is delivered.
| **[Home Connect Alt](https://github.com/ekutner/home-connect-hass)** | to integrate my dishwasher, I like this better than the [official integration](https://www.home-assistant.io/integrations/home_connect).
| **[ICS Calendar](https://github.com/franc6/ics_calendar)** | to integrate my partners work calendar.
| **[Cleanmate](https://github.com/albinmedoc/ha-cleanmate)** | my own integration to be able to controll my vacuum cleaner.

Actual secrets and auto-generated sensitive files are obviously kept off this repo! 😉

## License 📃

- Code and configuration is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).
- Documentation is licensed under the Creative Commons [Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0) License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Thanks 💕

Kudos to:

- **The [dedicated core team](https://www.home-assistant.io/blog)** that builds and manages Home Assistant. They work fast and humbly.
- **The horde of volunteer developers** of all components and add-ons.
- **The [vibrant community](https://community.home-assistant.io)**, always willing to help and share code samples.

Thank you for all your dedication, helpfulness and valuable insights. Cheers! 🍻😃

<p align="center"><strong>Don't forget to ⭐️ this repo! 😃</strong></p>

[badge-license]:https://img.shields.io/github/license/albinmedoc/homeassistant-config.svg?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48IURPQ1RZUEUgc3ZnIFBVQkxJQyAiLS8vVzNDLy9EVEQgU1ZHIDEuMS8vRU4iICJodHRwOi8vd3d3LnczLm9yZy9HcmFwaGljcy9TVkcvMS4xL0RURC9zdmcxMS5kdGQiPjxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgdmVyc2lvbj0iMS4xIiB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZD0iTTE3LjgsMjBDMTcuNCwyMS4yIDE2LjMsMjIgMTUsMjJINUMzLjMsMjIgMiwyMC43IDIsMTlWMThINUwxNC4yLDE4QzE0LjYsMTkuMiAxNS43LDIwIDE3LDIwSDE3LjhNMTksMkMyMC43LDIgMjIsMy4zIDIyLDVWNkgyMFY1QzIwLDQuNCAxOS42LDQgMTksNEMxOC40LDQgMTgsNC40IDE4LDVWMThIMTdDMTYuNCwxOCAxNiwxNy42IDE2LDE3VjE2SDVWNUM1LDMuMyA2LjMsMiA4LDJIMTlNOCw2VjhIMTVWNkg4TTgsMTBWMTJIMTRWMTBIOFoiIGZpbGw9IiNmZmZmZmYiIC8+PC9zdmc+Cg==&maxAge=86400


[link-board]:https://github.com/users/albinmedoc/projects/2
[link-issues]:https://github.com/albinmedoc/homeassistant-config/issues
[link-license]:LICENSE.md