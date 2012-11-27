# Repo setup

Upstream remote (origin): https://android.googlesource.com/platform/packages/inputmethods/LatinIME @jb-release

Requires Android framework packages:
* inputmethodcommon: https://android.googlesource.com/platform/frameworks/opt/inputmethodcommon @jb-release
* support (from SDK)

# Compiling
1. Create a symlink to inputmethodcommon
2. Create a symlink to jni folder in java source root
3. Set up NDK project: in Eclipse > Android Tools > Add Native Support...
4. Set up Support library: in Eclipse > Android Tools > Add Support Library...
5. Build native source, then Android app

# Branches

* **develop**: main development branch (all feature/bug branches should pull from here)
* **[version]-release**: version release branches (do not fork!)
