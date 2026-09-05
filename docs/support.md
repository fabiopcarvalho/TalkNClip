# Support

Start with the [getting started guide](getting-started.md). For a reproducible problem or a feature suggestion, open the **Issues** tab of this repository and choose the matching template. Reports in English or Portuguese are welcome.

## Common problems

| Symptom | What to check |
| --- | --- |
| Waiting for OBS Studio | Open OBS, enable its WebSocket server, and confirm that the port and password match TalkNClip settings. |
| Replay is not ready | Enable and start the Replay Buffer in OBS. Connecting TalkNClip alone does not start the buffer. |
| Microphone unavailable | Reconnect the selected microphone or explicitly select another one in Settings. Check Windows microphone access for desktop apps. |
| Microphone signal appears but no command runs | Confirm the recognition language and installed model, save a supported phrase, then use Voice Test. Check confidence and cooldown feedback. |
| A phrase contains unsupported words | Choose words supported by the selected speech model and resolve the validation message before saving. |
| Voice control is paused | Use Resume voice control in the tray menu. Manual recording controls remain available while paused. |
| Clips have missing audio | Check OBS audio sources, mixer, recording tracks, and output device. TalkNClip does not configure or mix recording audio. |
| License activation fails | Check your connection and the build's activation instructions. Record the error message without sharing the license key. |
| I started TalkNClip but can't see it | Check the Windows notification area and hidden tray icons. TalkNClip runs in the tray; starting a second instance does not open another controller. |

## Report a bug

Include the TalkNClip build/version, Windows and OBS versions, recognition language, steps to reproduce, expected result, and actual result. For voice issues, include the configured phrase if you are comfortable sharing it and say whether Voice Test recognizes it.

Provide the approximate time of the problem and relevant screenshots when useful. Crop or redact personal information, OBS passwords, license keys, and private file paths before posting.

## Diagnostics

Use **Voice Test** to separate microphone input and recognition from OBS actions. Wait until its calibration is complete before speaking. The top microphone indicator shows physical input; it does not by itself confirm that a command was accepted.

If more detail is needed, inspect the application's troubleshooting controls and local logs in `%LOCALAPPDATA%\VoiceObsController\Logs`. Normal logs omit speech transcripts. Optional diagnostic speech logging records recognized text locally, so enable it only when you intend to collect that information.

When using the support-package feature, review the preview and the resulting local ZIP before sharing it. Creating the package does not send it to anyone.

## Sensitive reports

Do not post license keys, passwords, payment details, or security exploit details in a public issue. For license or purchase-specific help, use the private contact channel supplied with your purchase or beta invitation. For a security issue, use private vulnerability reporting if this repository offers it, or an existing private maintainer contact.

Read [privacy and local data](privacy.md) for details about stored information and network access.
