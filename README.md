# Repo setup

Upstream remote (origin): https://android.googlesource.com/platform/packages/inputmethods/LatinIME @jb-release

Requires Android framework packages:
* inputmethodcommon: https://android.googlesource.com/platform/frameworks/opt/inputmethodcommon @jb-release
* support (from SDK)

# Compiling in Linux Eclipse 
1. Create a symlink to inputmethodcommon
2. Create a symlink to jni folder in java source root
3. Set up NDK project: in Eclipse > Android Tools > Add Native Support...
4. Set up Support library: in Eclipse > Android Tools > Add Support Library...
5. Build native source, then Android app

# Compiling in Windows Eclipse 
1. Remove \java\src\com\android\inputmethodcomm and \java\jni if they exist
2. Set up a linked folder to the source code in InputMethodCommon 
	a. Right click on src and choose New => Folder
	b. Type "internal" for Folder Name 
	c. Choose Advanced => Link to alternative location, and create a variable with name "LINKEDFOLDER_IMC" and set the variable to the location of java in InputMethodCommon 
3. Set up a linked folder to jni
	a. Right click the SettingsActivity and choose New => Folder
	b. Type "jni" for Folder Name 
	c. Choose Advanced => Link to alternative location, and create a variable with name "LINKEDFOLDER_JNI" and set the variable to \native\jni
4. Set up NDK project: in Eclipse > Android Tools > Add Native Support...
5. Set up Support library: in Eclipse > Android Tools > Add Support Library...
6. Build native source, then Android app

# Branches

* **develop**: main development branch (all feature/bug branches should pull from here)
* **[version]-release**: version release branches (do not fork!)
