% Download - microG Project
%
%

Download
--------
These page provides details to download sources for APK files from the microG Project.
For non-APK components, please consult the corresponding documentation.

### F-Droid repository
The best method to download and update components of the microG Project is to use our F-Droid repositories.
It currently provides stable and nightly updates for GmsCore as well as releases of GsfProxy and FakeStore.

[](id:mainrepo)
> %fdroid-repo-desc%
> > %row%
> > > %col-md-7%
> > > [Name](class:key) [microG F-Droid repo](class:val)
> > > [Address](class:key) [[https://microg.org/fdroid/repo](https://microg.org/fdroid/repo?fingerprint=9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165)](class:val)
> > > [Fingerprint of the signing key (SHA-256)](class:key) [9B D0 67 27 E6 27 96 C0 13 0E B6 DA B3 9B 73 15 74 51 58 2C BD 13 8E 86 C4 68 AC C3 95 D1 41 65](class:val)
> >
> > > %col-md-5%
> > > [<img src="https://chart.googleapis.com/chart?cht=qr&chl=https%3A%2F%2Fmicrog.org%2Ffdroid%2Frepo%3Ffingerprint%3D9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165&chs=256x256&choe=UTF-8&chld=L|0">](https://microg.org/fdroid/repo?fingerprint=9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165)

### Direct downloads
Nonetheless we provide direct downloads of apk files.

[](id:app_com_google_android_gms)
> %fdroid-dl-app%
> > %row%
> > > %col-sm-1%
> > > <img src="/img/gmscore_96px.png" height="48">
> >
> > > %col-sm-8%
> > > [microG Services Core](class:name) [com.google.android.gms](class:pname)
> >
> > > %col-sm-3%
> > > > %btn-group%
> > > > <a href="https://github.com/microg/android_packages_apps_GmsCore/releases" class="btn btn-default btn-dl">Download stable [via GitHub](class:ver)</a>

[](id:app_com_google_android_gsf)
> %fdroid-dl-app%
> > %row%
> > > %col-sm-1%
> > > <img src="/img/gmscore_96px.png" height="48">
> >
> > > %col-sm-8%
> > > [microG Services Framework Proxy](class:name) [com.google.android.gsf](class:pname)
> >
> > > %col-sm-3%
> > > > %btn-group%
> > > > <a href="https://github.com/microg/android_packages_apps_GsfProxy/releases" class="btn btn-default btn-dl">Download stable [via GitHub](class:ver)</a>

[](id:app_com_android_vending)
> %fdroid-dl-app%
> > %row%
> > > %col-sm-1%
> > > <img src="/img/store_96px.png" height="48">
> >
> > > %col-sm-8%
> > > [microG Store (FakeStore release)](class:name) [com.android.vending](class:pname)
> >
> > > %col-sm-3%
> > > > %btn-group%
> > > > <a href="https://github.com/microg/android_packages_apps_FakeStore/releases" class="btn btn-default btn-dl">Download stable [via GitHub](class:ver)</a>

[](id:app_org_microg_unifiednlp)
> %fdroid-dl-app%
> > %row%
> > > %col-sm-1%
> > > <img src="/img/unifiednlp_96px.png" height="48">
> >
> > > %col-sm-8%
> > > [microG UnifiedNlp](class:name) [org.microg.unifiednlp](class:pname)
> >
> > > %col-sm-3%
> > > > %btn-group%
> > > > <a href="https://github.com/microg/android_packages_apps_UnifiedNlp/releases" class="btn btn-default btn-dl">Download stable [via GitHub](class:ver)</a>

[](id:app_com_google_android_maps)
> %fdroid-dl-app%
> > %row%
> > > %col-sm-1%
> > > <img src="/img/gmscore_96px.png" height="48">
> >
> > > %col-sm-8%
> > > [microG Maps API v1](class:name) [com.google.android.maps](class:pname)
> >
> > > %col-sm-3%
> > > > %btn-group%
> > > > <a href="https://github.com/microg/android_frameworks_mapsv1/releases" class="btn btn-default btn-dl">Download stable [via GitHub](class:ver)</a>

<script src="/js/jquery-2.2.1.min.js"></script>
<script src="/js/fdroid.js"></script>
<script type="text/javascript">
    fdroid.getRepoInfo("https://microg.org/fdroid/repo", function(repoInfo) {
        $("#mainrepo").parent().next().children(".row").replaceWith(fdroid.createRepoDetails(repoInfo));
        ["com.google.android.gms", "com.google.android.gsf", "com.android.vending"].forEach(function(name) {
            $("#app_"+name.split(".").join("_")).parent().next().children(".row").children().children(".btn-group")
                .replaceWith(fdroid.createDownloadButton(repoInfo, name));
        });
    });
</script>
