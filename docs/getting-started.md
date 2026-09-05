# Getting started

## 1. Prepare your setup

Have the following ready:

- A Windows x64 PC and a microphone available to Windows desktop applications.
- OBS Studio with obs-websocket 5.x support. OBS Studio 28 and later include the WebSocket server.
- A TalkNClip package and its accompanying installation instructions.
- Internet access to download your speech model and, for builds that require a license, complete initial activation.

Follow the installation and licensing instructions supplied with your build, and keep the application package intact. If your package requires the .NET Desktop Runtime, install the version specified in those instructions. The current portable Beta uses the executable name `VoiceObsController.exe`.

## 2. Connect OBS Studio

1. Open OBS Studio.
2. Open **Tools → WebSocket Server Settings**.
3. Enable the WebSocket server and configure a password.
4. Start TalkNClip and open **Settings** from its notification area icon.
5. Enter the matching OBS connection settings and password. The default connection is to the same PC on port `4455`.
6. Save and check that TalkNClip shows OBS as connected.

TalkNClip waits for OBS when it is closed and attempts to reconnect when it becomes available.

## 3. Prepare recording and instant clips

Configure your scenes, recording output folder, video settings, and audio sources in OBS. Make a short recording in OBS to confirm that the intended picture and audio are present.

For instant clips, enable **Replay Buffer** in OBS output settings, choose how many seconds to keep, and start the Replay Buffer. TalkNClip must show replay as ready before it can save a clip.

TalkNClip uses the audio mix configured in OBS. Its microphone selection is for recognizing voice commands; it does not add that microphone to your recording. A configured audio source does not guarantee that it currently has an audible signal.

## 4. Set up your voice

1. Follow the first-run setup or open **Settings**.
2. Select your microphone explicitly.
3. Choose **Portuguese (Brazil)** or **English (United States)** as the recognition language. The interface language is a separate preference.
4. Download the offered speech model if it is not installed. Recognition works locally after installation.
5. Open **Voice Commands** and choose phrases for saving a clip, starting recording, and stopping recording. Enter additional phrases on separate lines.
6. Resolve any unsupported-word or conflicting-phrase messages, then save.

Use the phrases displayed in your selected language profile. Speak the complete configured phrase; TalkNClip recognizes a configured set of commands rather than general conversation.

## 5. Test before recording

Open **Voice Test** or use **Test** beside a command. Stay quiet during the initial noise calibration, then say the phrase when the test indicates it is ready.

Voice Test does not execute OBS actions by default. Check the recognized phrase and result. The optional five-attempt reliability test also runs without OBS actions.

In **Show voice detection**, the top indicator represents microphone signal. A command indicator represents a recognized configured phrase. Confidence and cooldown checks still determine whether an action can be sent to OBS.

## 6. Use TalkNClip

With voice control enabled and OBS ready, say a saved command. Confirm the recording or saved clip in OBS. Clip length and file location follow your OBS configuration.

The tray menu provides manual controls, including **Save clip now** when replay is ready and **Stop recording** while recording. **Pause voice control** stops normal voice listening while leaving OBS and manual controls available; **Resume voice control** restores listening.

When you exit TalkNClip, it attempts to stop a recording it started. A recording already active when TalkNClip connected is not automatically taken over. Confirm recording status in OBS before closing your setup.

For connection, microphone, or recognition problems, see [support](support.md).
