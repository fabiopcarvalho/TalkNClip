# Third-party notices

TalkNClip uses third-party software for local speech recognition, microphone access, and its Windows application runtime. This page summarizes the current project inventory; exact components can vary by application package.

## Component acknowledgments

| Component | Recorded version | Recorded license | Role |
| --- | --- | --- | --- |
| Vosk | 0.3.38 | Apache-2.0 | Offline speech recognition. Copyright Alpha Cephei Inc. |
| NAudio and its transitive NAudio packages | 3.0.1 | MIT | Microphone access and audio handling. Copyright Mark Heath and contributors. |
| System.Numerics.Tensors | 9.0.0 | MIT | Transitive application dependency. Copyright Microsoft Corporation. |
| GNU libgcc and libstdc++ runtimes | GCC 8.3.0; Debian `8.3.0-6+21.3~deb10u2` | GPL-3.0 with GCC Runtime Library Exception 3.1 | Native runtime DLLs supplied through Vosk 0.3.38. Corresponding Source access is provided with the application package. |
| MinGW-w64 winpthreads runtime | 6.0.0-3 | MinGW-w64 runtime terms | Native POSIX threads runtime supplied through Vosk 0.3.38. |
| Microsoft .NET and Windows Desktop Runtime | 10.0.12 | Microsoft distribution license plus component third-party terms | Self-contained Windows application runtime. |
| Vosk Small Portuguese model | 0.3 | Apache-2.0, as recorded in the model manifest | Portuguese speech recognition; downloaded separately. |
| Vosk Small English US model | 0.15 | Apache-2.0, as recorded in the model manifest | English speech recognition; downloaded separately. |
| Vosk Small Spanish model | 0.42 | Apache-2.0, as recorded in the model manifest | Spanish speech recognition; downloaded separately. |
| Vosk Small German model | 0.15 | Apache-2.0, as recorded in the model manifest | German speech recognition; downloaded separately. |
| Vosk Small Italian model | 0.22 | Apache-2.0, as recorded in the model manifest | Italian speech recognition; downloaded separately. |
| Vosk Small French model | 0.22 | Apache-2.0, as recorded in the model manifest | French speech recognition; downloaded separately. |

OBS Studio is the separately installed recording application that TalkNClip controls through OBS WebSocket.

## Package notices

Refer to the `THIRD-PARTY-NOTICES.txt` and `licenses` directory supplied with an application package for its included notices and license texts. This summary does not replace those materials or grant a license to TalkNClip itself.

The package reviewed for this page is:

| Package property | Verified value |
| --- | --- |
| Microsoft Store package version | `1.0.1.0` |
| Architecture | Windows x64 |
| Deployment | Self-contained |
| MSIX size | 99,123,525 bytes |
| MSIX SHA-256 | `97a027021f3927da30d3d658ab973f332c0a00ef2ed9a27e04025dd84a08e76e` |
| Audited contents | 535 files; 239,887,368 uncompressed bytes |

The reviewed Microsoft Store package is self-contained and includes .NET
10.0.12. It carries the matching `dotnet/runtime` and `dotnet/wpf` license and
third-party notice files.

## Distribution notice status

The licensing and notice review is complete for Microsoft Store package
`1.0.1.0`. The exact native files were identified by SHA-256 and byte-for-byte
comparison with official historical Debian packages:

| Distributed file | Verified origin | SHA-256 |
| --- | --- | --- |
| `libgcc_s_seh-1.dll` | Debian `gcc-mingw-w64-x86-64` `8.3.0-6+21.3~deb10u2`, POSIX model | `e16de83d48247cde2581ec36279102dda00b7d7b36558cad72164e3c4caae0a4` |
| `libstdc++-6.dll` | Debian `g++-mingw-w64-x86-64` `8.3.0-6+21.3~deb10u2`, POSIX model | `1766f6e252410086c26400ab085e017e7ad5e8993f3d19dda87a13a1e978f0a2` |
| `libwinpthread-1.dll` | Debian `mingw-w64-x86-64-dev` `6.0.0-3` | `5b60907df42009f1ba437e7f2a6278651be97f4993869105d8a31086138e4570` |

The package reproduces GPL-3.0, the GCC Runtime Library Exception 3.1, the
exact MinGW-w64 6.0.0 runtime notices, and directions with checksums for
accessing the complete GCC and MinGW Corresponding Source under GPL-3.0
section 6(d). See [GCC runtime Corresponding Source](gcc-corresponding-source.md)
for the exact source archives, sizes, SHA-256 values, and signed Debian source
manifests. The source is available through the historical Debian Snapshot
archive at no charge.

The license exception permits TalkNClip and Vosk to use the GCC runtime
libraries without changing the licenses of their independent code. The source
access provision covers the separate GPL runtime DLLs themselves.

Official references:

- [Vosk 0.3.38 source and Windows build recipe](https://github.com/alphacep/vosk-api/tree/v0.3.38)
- [GNU libstdc++ license](https://gcc.gnu.org/onlinedocs/libstdc++/manual/license.html)
- [GCC Runtime Library Exception FAQ](https://www.gnu.org/licenses/gcc-exception-3.1-faq.html)
- [GPL-3.0 section 6](https://www.gnu.org/licenses/gpl-3.0.html#section6)
- [Debian gcc-mingw-w64 source `21.3~deb10u2`](https://snapshot.debian.org/package/gcc-mingw-w64/21.3~deb10u2/)
- [Debian GCC source `8.3.0-6`](https://snapshot.debian.org/package/gcc-8/8.3.0-6/)
- [Debian MinGW-w64 source `6.0.0-3`](https://snapshot.debian.org/package/mingw-w64/6.0.0-3/)
- [.NET 10.0.12 downloads](https://dotnet.microsoft.com/en-us/download/dotnet/10.0)
- [.NET distribution packaging guidance](https://learn.microsoft.com/en-us/dotnet/core/distribution-packaging)
