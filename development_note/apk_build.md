# How to build an APK

`javac` compile `R.java` + `aidl` files + Android Java classes to Java `.class` bytecode. Then use `dx` tool to convert them to `.dex` [Dalvik EXecutable](https://stackoverflow.com/questions/7750448/what-are-dex-files-in-android) bytecode files. Then `aapt` packaging compile resources into binary assets and put to `APK Packager`. `APK packager` use bytecode, resources and signed keystore to build APK.