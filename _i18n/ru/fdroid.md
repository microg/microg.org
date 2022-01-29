% Репозиторий F-Droid - Проект microG
%
%

Репозиторий F-Droid
-------------------
Официальные репозитории приложений от проекта microG.


[](id:mainrepo)
> %fdroid-repo-desc%
> > %row%
> > > %col-md-7%
> > > [Название](class:key) [microG F-Droid repo](class:val)
> > > [Адрес](class:key) [[https://microg.org/fdroid/repo](https://microg.org/fdroid/repo?fingerprint=9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165)](class:val)
> > > [Отпечаток ключа подписи (SHA-256)](class:key) [9B D0 67 27 E6 27 96 C0 13 0E B6 DA B3 9B 73 15 74 51 58 2C BD 13 8E 86 C4 68 AC C3 95 D1 41 65](class:val)
> >
> > > %col-md-5%
> > > [<img src="https://chart.googleapis.com/chart?cht=qr&chl=https%3A%2F%2Fmicrog.org%2Ffdroid%2Frepo%3Ffingerprint%3D9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165&chs=256x256&choe=UTF-8&chld=L|0">](https://microg.org/fdroid/repo?fingerprint=9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165)


[](id:archiverepo)
> %fdroid-repo-desc%
> > %row%
> > > %col-md-7%
> > > [Название](class:key) [microG F-Droid archive](class:val)
> > > [Адрес](class:key) [[https://microg.org/fdroid/archive](https://microg.org/fdroid/archive?fingerprint=9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165)](class:val)
> > > [Отпечаток ключа подписи (SHA-256)](class:key) [9B D0 67 27 E6 27 96 C0 13 0E B6 DA B3 9B 73 15 74 51 58 2C BD 13 8E 86 C4 68 AC C3 95 D1 41 65](class:val)
> >
> > > %col-md-5%
> > > [<img src="https://chart.googleapis.com/chart?cht=qr&chl=https%3A%2F%2Fmicrog.org%2Ffdroid%2Farchive%3Ffingerprint%3D9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165&chs=256x256&choe=UTF-8&chld=L|0">](https://microg.org/fdroid/archive?fingerprint=9BD06727E62796C0130EB6DAB39B73157451582CBD138E86C468ACC395D14165)

<script src="/js/fdroid.js"></script>
<script type="text/javascript">
    fdroid.getRepoInfo("https://microg.org/fdroid/repo", function(repoInfo) {
        $("#mainrepo").parent().next().children(".row").replaceWith(fdroid.createRepoDetails(repoInfo));
    });
    fdroid.getRepoInfo("https://microg.org/fdroid/archive", function(repoInfo) {
        $("#archiverepo").parent().next().children(".row").replaceWith(fdroid.createRepoDetails(repoInfo));
    });
</script>
