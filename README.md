# Repo setup

Upstream remote (origin): https://android.googlesource.com/platform/packages/inputmethods/LatinIME @jb-release

Relies on the following framework packages:
* inputmethodcommon: symlink to https://android.googlesource.com/platform/frameworks/opt/inputmethodcommon @jb-release
* support: in Eclipse > Android Tools > Add support library...

## Branches

* **develop**: main development branch (all feature/bug branches should pull from here)
* **[version]-release**: version release branches (do not fork!)
* **jb-release**: original branch (do not fork!)

## Getting Here

1. Renamed package to ca.idrc.tecla
1. Search and replaced original namespace references from com.android.inputmethod.<endpoint> to ca.idrc.tecla.<endpoint>
1. Renamed native code files and package references to reflect updated namespace (search & replace com.android... com/android... com_android...)
1. Removed -Werror flag from Android.mk NDK file
