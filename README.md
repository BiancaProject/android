Bianca Project
==============

Getting started
---------------

To get started with Bianca Project, you'll need to get
familiar with [Repo](https://source.android.com/source/using-repo.html) and [Version Control with Git](https://source.android.com/source/version-control.html).

To initialize your local repository using the Bianca Project trees, use a command like this:
```
repo init -u https://github.com/BiancaProject/android.git -b 13
```
Then to sync up:
```
repo sync --force-sync --no-tags --no-clone-bundle
```

To build, use command:
```
source build/envsetup.sh
lunch $device-userdebug
m dudu
```

To build signed, use command:
```
source build/envsetup.sh
keygen
lunch $device-user
m dudu-sign
```

After creating the keys with `keygen`, you won't need to do it again. Just make sure to backup directory called certs inside the rom root directory.

Credits:
========
 * [**Proton AOSP**](https://github.com/ProtonAOSP)
 * [**Lineage OS**](https://github.com/LineageOS)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**Nusantara ROM**](https://github.com/Nusantara-ROM)
 * [**Project Sakura**](https://github.com/ProjectSakura)
 * [**DerpFest-11**](https://github.com/DerpFest-11)
 * [**exTHmUI**](https://github.com/exthmui)
