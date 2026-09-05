# Third-party notices

TalkNClip uses third-party software for local speech recognition, microphone access, and its Windows application runtime. This page summarizes the current project inventory; exact components can vary by application package.

## Component acknowledgments

| Component | Recorded version | Recorded license | Role |
| --- | --- | --- | --- |
| Vosk | 0.3.38 | Apache-2.0 | Offline speech recognition. Copyright Alpha Cephei Inc. |
| NAudio and its transitive NAudio packages | 3.0.1 | MIT | Microphone access and audio handling. Copyright Mark Heath and contributors. |
| System.Numerics.Tensors | 9.0.0 | MIT | Transitive application dependency. Copyright Microsoft Corporation. |
| Vosk Small Portuguese model | 0.3 | Apache-2.0, as recorded in the model manifest | Portuguese speech recognition; downloaded separately. |
| Vosk Small English US model | 0.15 | Apache-2.0, as recorded in the model manifest | English speech recognition; downloaded separately. |

OBS Studio is the separately installed recording application that TalkNClip controls through OBS WebSocket.

## Package notices

Refer to the `THIRD-PARTY-NOTICES.txt` and `licenses` directory supplied with an application package for its included notices and license texts. This summary does not replace those materials or grant a license to TalkNClip itself.

Self-contained packages also include the .NET runtime and need the corresponding runtime license and third-party notices. Framework-dependent packages use a separately installed runtime.

## Distribution notice status

The current project inventory still records unresolved provenance and notice requirements for the Vosk-supplied native files `libgcc_s_seh-1.dll`, `libstdc++-6.dll`, and `libwinpthread-1.dll`. It also records pending matching .NET runtime notices for self-contained packages.

Those package-specific items must be resolved before public binary distribution. Publishing this documentation does not indicate that a binary package has completed that review.
