<p align="center">
  <img src="assets/banner.png" alt="TalkNClip" width="900">
</p>

<h1 align="center">TalkNClip</h1>

<p align="center">
  <strong>Say it. Clip it.</strong>
</p>

<p align="center">
  Voice-controlled instant replay and recording for OBS Studio on Windows.
</p>

TalkNClip lets you save an instant clip, start recording, and stop recording with your voice. It runs in the Windows notification area and sends your configured commands to OBS Studio.

## What you can do

- Save the last moments captured by the OBS Replay Buffer.
- Start and stop OBS recordings with custom voice phrases.
- Recognize commands locally in Portuguese (Brazil) or English (United States).
- Test your phrases before using them to control OBS.
- Check OBS, microphone, recording, and replay status from the tray.
- Pause voice control while keeping manual recording and clip controls available.
- Choose a light or dark settings window.

OBS handles recording, audio mixing, replay duration, and output files. Configure your scenes and audio sources in OBS as usual.

## Get started

You need a Windows x64 PC, a microphone, OBS Studio with WebSocket support enabled, and a speech model for your selected language. Saving instant clips also requires the OBS Replay Buffer to be running.

Follow the [getting started guide](docs/getting-started.md) to connect OBS and test your first command. Installation and licensing requirements depend on the build you receive; follow the instructions supplied with that package.

## Screenshots

### Settings

![TalkNClip settings](assets/screenshots/settings.png)

### Voice commands

![Custom voice commands](assets/screenshots/voice-commands.png)

### Voice test

![Testing a voice command](assets/screenshots/voice-test.png)

### Tray controls

![TalkNClip notification area menu](assets/screenshots/tray.png)

## Privacy

Speech recognition runs locally on your selected microphone. TalkNClip does not upload microphone audio or use cloud speech recognition. Model downloads and license activation or validation can require an internet connection.

Read [privacy and local data](docs/privacy.md) for details about network access, logs, and support packages.

## Help and feedback

See the [support guide](docs/support.md) for troubleshooting and how to report a problem through this repository's Issues tab.

This repository hosts the public documentation, screenshots, and issue templates for TalkNClip. Application source code is maintained separately.

See [third-party notices](docs/third-party-notices.md) for component acknowledgments and the status of distribution notices.

Created by Fabio Carvalho.
