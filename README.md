# BoomBeastic mini

A Raspberry Pi Zero based smart connected speaker based on [Mopidy](https://github.com/mopidy/mopidy)!

## Parts list

#### rpi2/2+/3 version
please refer to [this link](https://github.com/resin-io-playground/boombeastic/blob/master/docs/v1/mini/rpi3/bom.md)
#### rpi0 version
please refer to [this link](https://github.com/resin-io-playground/boombeastic/blob/master/docs/v1/mini/rpi0/bom.md)

## Assembly

#### rpi2/2+/3 version
please refer to [this link](https://github.com/resin-io-playground/boombeastic/blob/master/docs/v1/mini/rpi3/assembly.md)
#### rpi0 version
please refer to [this link](https://github.com/resin-io-playground/boombeastic/blob/master/docs/v1/mini/rpi0/assembly.md)

## Getting started

- Sign up on [resin.io](https://dashboard.resin.io/signup)
- go throught the [getting started guide](http://docs.resin.io/raspberrypi/nodejs/getting-started/) and create a new RPI zero application called `boombeasticmini`
- clone this repository to your local workspace
- set these environment variables in the `Fleet Configuration` application side tab

  - `RESIN_HOST_CONFIG_dtoverlay` = `hifiberry-dac`

- add the _resin remote_ to your local workspace using the useful shortcut in the dashboard UI ![remoteadd](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/gitresinremote.png)
- `git push resin master`
- see the magic happening, your device is getting updated Over-The-Air!

## Configure via [environment variables](https://docs.resin.io/management/env-vars/)
Variable Name | Default | Description
------------ | ------------- | -------------
MOPIDY_HTTP_PORT | `8080` | the port on which expose the web UI
MOPIDY_MPD_PORT | `6680` | the port on which expose the MPD service
MOPIDY_AUDIO_MIXER_VOLUME | `50` | the default volume
MOPIDY_GMUSIC_ENABLED | `false` | if set `true` loads the [Google Play Music extension](https://github.com/mopidy/mopidy-gmusic)
MOPIDY_GMUSIC_USERNAME | `none` | your Google username
MOPIDY_GMUSIC_PASSWORD | `none` | your Google Play Music password (an [app password](https://support.google.com/accounts/answer/185833) is suggested as a best practice)
MOPIDY_GMUSIC_ALL_ACCESS | `false` | if set `true` configures the extension for handling the All Access subscription
MOPIDY_SPOTIFY_ENABLED | `false` | if set `true` loads the [Spotify extension](https://github.com/mopidy/mopidy-spotify)
MOPIDY_SPOTIFY_USERNAME | `none` | your Spotify username
MOPIDY_SPOTIFY_PASSWORD | `none` | your Spotify password
MOPIDY_SOUNDCLOUD_ENABLED | `false` | if set `true` loads the [SoundCloud extension](https://github.com/mopidy/mopidy-soundcloud)
MOPIDY_SOUNDCLOUD_AUTH_TOKEN | `none` | your SoundCloud [token](https://www.mopidy.com/authenticate/)
MOPIDY_YOUTUBE_ENABLED | `false` | if set `true` loads the [YouTube extension](https://github.com/mopidy/mopidy-youtube)

## Videos

* [video1](https://www.youtube.com/watch?v=EnLgmW8kyis)

## Pictures

![v1_rpi3_1](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/v1/mini/rpi3/photos/IMG_20160929_163629.jpg)

---

![v1_rpi3_2](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/v1/mini/rpi3/photos/IMG_20160929_163751.jpg)

---

![v1_rpi3_3](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/v1/mini/rpi3/photos/IMG_20161004_170024.jpg)

---

![v1_stereo](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/v1/mini/rpi0/photos/20160712_005947.jpg)

---

![v1_mono](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/v1/mini/rpi0/photos/20160711_222357.jpg)

---

![v1_battery](https://raw.githubusercontent.com/resin-io-playground/boombeastic/master/docs/v1/mini/rpi0/photos/20160712_150552.jpg)

## License

Copyright 2016 Resinio Ltd.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
