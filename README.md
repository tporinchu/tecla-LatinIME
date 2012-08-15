# Repo setup

Upstream remote (origin): https://android.googlesource.com/platform/packages/inputmethods/LatinIME @jb-release

Relies on symlinks to Android framework packages:
* inputmethodcommon: https://android.googlesource.com/platform/frameworks/opt/inputmethodcommon @jb-release
* support: https://android.googlesource.com/platform/frameworks/support @jb-release

## Branches

* **develop**: main development branch (all feature/bug branches should pull from here)
* **[version]-release**: version release branches (do not fork!)
* **jb-release**: original branch (do not fork!)

## Getting Here

1. Renamed package to ca.idrc.tecla
1. Search and replaced original namespace references from com.android.inputmethod.<endpoint> to ca.idrc.tecla.<endpoint>
1. Renamed native code files and package references to reflect updated namespace (e.g., ProximityInfo, BinaryDictionary)
1. Removed -Werror flag from Android.mk NDK file
