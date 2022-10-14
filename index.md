% microG Project
%
%

> %jumbotron%
> # <img src="/img/microg_full_colored.svg" alt="microG"> Project
> ### A free-as-in-freedom re-implementation of Google's proprietary Android user space apps and libraries.

About
-----
The linux-based open-source mobile operating system Android is not only the most popular mobile operating system in the world, 
it's also on the way to becoming a proprietary operating system. How is that?

While the core operating system is still released as part of the Android Open Source Project, the majority of core apps are not.
It gets worse: More and more libraries and APIs are only available on phones that run various Google apps pre-installed,
effectively locking third-party apps to the Google ecosystem. For these reasons Android is [described as being](https://arstechnica.com/gadgets/2018/07/googles-iron-grip-on-android-controlling-open-source-by-any-means-necessary/) a "*look but don't touch*" kind of open.

At this point, several popular open-source applications like the [secure messenger Signal](https://github.com/WhisperSystems/Signal-Android) already require some of Google's proprietary libraries to be installed. 
Increasing demand in the free software community in addition to severe problems in Google's proprietary software discovered by the Android modding community, have led to the development of a free software clone of Google's proprietary core libraries and applications - the microG Project was born.

Although most microG components are far from complete, users are amazed by the results. Free software users got extended application support,
privacy-caring users can reduce or monitor data that is sent to Google and especially older phones can expect some battery life improvements.
microG is not only used on real devices, but also replaces Google tools in test emulators and is even used in virtual mobile infrastructure.

Components
----------
- **Service Core (GmsCore)** is a library app, providing the functionality required to run apps that use Google Play Services or Google Maps Android API (v2).
  
  [More details and installation instructions](https://github.com/microg/android_packages_apps_GmsCore/wiki)
- **Services Framework Proxy (GsfProxy)** is a small helper utility to allow apps developed for Google Cloud to Device Messaging (C2DM) to use the compatible Google Cloud Messaging service included with GmsCore.

  [Read GmsCore documentation for details](https://github.com/microg/android_packages_apps_GmsCore/wiki)
- **Unified Network Location Provider (UnifiedNlp)** is a library that provides Wi-Fi- and Cell-tower-based geolocation to applications that use Google's network location provider.
  It is included in GmsCore but can also run independently on most Android systems.
  
  [More details and installation instructions](https://github.com/microg/android_packages_apps_UnifiedNlp/blob/master/README.md)
- **Maps API (mapsv1)** is a system library, providing the same functionality as now deprecated Google Maps API (v1).

  [More details and installation instructions](https://github.com/microg/android_frameworks_mapsv1)
- **Store (Phonesky)** is a frontend application providing access to the Google Play Store to download and update applications. Development is in early stage and there is no usable application yet.
