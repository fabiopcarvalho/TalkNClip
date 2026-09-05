# Privacy and local data

This page describes the implemented behavior of the current TalkNClip application. Package-specific instructions may describe differences for the build you receive.

## Microphone and speech

TalkNClip captures the microphone you select and processes its audio locally with an installed Vosk speech model. It does not use cloud speech recognition, upload microphone audio, or capture system output audio for recognition.

If the selected microphone becomes unavailable, voice control stops instead of automatically switching devices. Pausing voice control releases the main microphone capture; opening Voice Test can use the microphone separately while normal voice control remains paused.

OBS is responsible for recordings and clips, including their audio, storage location, and contents.

## Network connections

| Purpose | Behavior |
| --- | --- |
| OBS control | Connects to the configured OBS WebSocket server, on `localhost:4455` by default. Advanced settings can change the destination. |
| Speech model installation | Downloads the selected model after an explicit user action and checks it against the application's recorded SHA-256 checksum. Subsequent speech recognition runs locally. |
| Licensing | Builds with licensing use the Lemon Squeezy License API for activation, validation, and deactivation. Requests include the license key and, as applicable, an installation name or license instance identifier. |

The application has no telemetry client or automatic support upload. Local speech recognition does not imply that all application features work without internet access: initial license activation requires a connection, and licensed builds perform periodic validation with a limited offline grace period.

## Settings and license data

Application data is stored under `%LOCALAPPDATA%\VoiceObsController`. This folder keeps the application's original technical name for compatibility.

- `settings.json` stores preferences, configured command phrases, microphone selection, and OBS connection settings.
- The OBS password is protected with Windows Data Protection API (DPAPI) for the current Windows user before storage.
- License data uses a local installation identifier and a DPAPI-protected payload for the license key, instance information, and validation cache.
- Installed speech models and application logs are stored locally.

Configured phrases are saved preferences. They are separate from transcripts of what the microphone recognized.

## Logs and diagnostics

Normal logs do not contain recognized speech text. **Diagnostic speech logging** is off by default; enabling it records recognized speech locally in the application log. Disable it after troubleshooting if you no longer need it.

Logs are stored in the application's `Logs` folder, with the 14 most recent log files retained.

A support package is created locally as a ZIP only after you request it and confirm its preview. The package excludes OBS passwords, DPAPI secrets, speech transcriptions, microphone audio, video, clips, and tokens. It is not sent automatically. Review any file or screenshot before choosing to share it.

## Removing local data

If needed, deactivate your license in the application before removing an installation. Close TalkNClip before deleting its local data folder. Removing that folder removes local settings, downloaded models, logs, and cached license data; it does not itself deactivate a server-side license instance or delete recordings stored by OBS.

Public issues and attachments are visible to other people. Do not post passwords, license keys, or private recordings. See the [support guide](support.md).
