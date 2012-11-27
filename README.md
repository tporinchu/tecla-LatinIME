# Repo setup

Upstream remote (origin): https://android.googlesource.com/platform/packages/inputmethods/LatinIME @jb-release

Relies on symlinks to Android framework packages:
* inputmethodcommon: https://android.googlesource.com/platform/frameworks/opt/inputmethodcommon @jb-release
* support: in Eclipse > Android Tools > Add support library...

## Branches

* **develop**: main development branch (all feature/bug branches should pull from here)
* **[version]-release**: version release branches (do not fork!)
