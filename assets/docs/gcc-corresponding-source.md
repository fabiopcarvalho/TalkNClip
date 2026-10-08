# GCC runtime Corresponding Source

Microsoft Store package `1.0.1.0` distributes the following independent object-code libraries received through Vosk 0.3.38:

| Distributed file | SHA-256 |
| --- | --- |
| `libgcc_s_seh-1.dll` | `e16de83d48247cde2581ec36279102dda00b7d7b36558cad72164e3c4caae0a4` |
| `libstdc++-6.dll` | `1766f6e252410086c26400ab085e017e7ad5e8993f3d19dda87a13a1e978f0a2` |
| `libwinpthread-1.dll` | `5b60907df42009f1ba437e7f2a6278651be97f4993869105d8a31086138e4570` |

The first two files match byte for byte the POSIX thread model DLLs in the official Debian `gcc-mingw-w64-x86-64` and `g++-mingw-w64-x86-64` packages, version `8.3.0-6+21.3~deb10u2`. They are GNU Compiler Collection 8.3.0 runtime libraries licensed under GPL-3.0 with the GCC Runtime Library Exception 3.1.

The exception permits independent programs to use these runtime libraries. It does not remove the GPL requirement to provide Corresponding Source when the runtime DLLs themselves are distributed in object-code form. TalkNClip provides equivalent network access to the complete machine-readable source and Debian build packaging under GPL-3.0 section 6(d), at no charge.

## GCC 8.3.0 source

| Source file | Size | SHA-256 |
| --- | ---: | --- |
| [gcc-8_8.3.0.orig.tar.gz](https://snapshot.debian.org/archive/debian/20190225T151539Z/pool/main/g/gcc-8/gcc-8_8.3.0.orig.tar.gz) | 87,764,363 bytes | `ee3fd608f66e5737f20cf71b176cfbf58f7c1d190ad6def33d57610cdae8eac2` |
| [gcc-8_8.3.0-6.diff.gz](https://snapshot.debian.org/archive/debian/20190406T212022Z/pool/main/g/gcc-8/gcc-8_8.3.0-6.diff.gz) | 704,334 bytes | `211e5e1022e115abbcb9eeb39cf4bf84958c4e8469c0cbe430569947a04c5415` |

[Signed Debian source manifest for GCC 8.3.0-6](https://snapshot.debian.org/archive/debian/20190406T212022Z/pool/main/g/gcc-8/gcc-8_8.3.0-6.dsc)

## Debian MinGW GCC cross-compiler build packaging

| Source file | Size | SHA-256 |
| --- | ---: | --- |
| [gcc-mingw-w64_21.3~deb10u2.tar.xz](https://snapshot.debian.org/archive/debian/20210807T203040Z/pool/main/g/gcc-mingw-w64/gcc-mingw-w64_21.3~deb10u2.tar.xz) | 57,896 bytes | `f1fad9a26ab6392cf127d9670a964254567dd5f0686a3936e7b6fd35648a909b` |

[Signed Debian source manifest for gcc-mingw-w64 21.3~deb10u2](https://snapshot.debian.org/archive/debian/20210807T203040Z/pool/main/g/gcc-mingw-w64/gcc-mingw-w64_21.3~deb10u2.dsc)

## MinGW-w64 6.0.0 source and Debian build packaging

These sources provide the target headers and runtime used to build the GCC runtime DLLs and the separately distributed `libwinpthread-1.dll`.

| Source file | Size | SHA-256 |
| --- | ---: | --- |
| [mingw-w64_6.0.0.orig.tar.bz2](https://snapshot.debian.org/archive/debian/20181024T215635Z/pool/main/m/mingw-w64/mingw-w64_6.0.0.orig.tar.bz2) | 9,045,653 bytes | `805e11101e26d7897fce7d49cbb140d7bac15f3e085a91e0001e80b2adaf48f0` |
| [mingw-w64_6.0.0-3.debian.tar.xz](https://snapshot.debian.org/archive/debian/20181112T040149Z/pool/main/m/mingw-w64/mingw-w64_6.0.0-3.debian.tar.xz) | 104,784 bytes | `1a925dc9b037516e420960b340985a9ead1bbe5cb6ad33dd39a3e7b2572de50c` |

[Signed Debian source manifest for MinGW-w64 6.0.0-3](https://snapshot.debian.org/archive/debian/20181112T040149Z/pool/main/m/mingw-w64/mingw-w64_6.0.0-3.dsc)

## Availability

TalkNClip is responsible for keeping this Corresponding Source available for as long as GPL-3.0 section 6 requires. If any link becomes unavailable, contact [talknclip.support@gmail.com](mailto:talknclip.support@gmail.com), and the same verified source archives will be made available at no charge.

See the [third-party notices](third-party-notices.md) for the complete package inventory and official license references.
