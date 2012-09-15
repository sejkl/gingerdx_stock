Build instructions:
===================

repo init -u git://github.com/TeamFun/android.git -b gingerbread
. build/envsetup.sh
lunch cyanogen_hero-eng
make -j6 update-api
make -j6

After build go to out directory and copy app and framework into these stock essentials.
Take a build.prop from shakira build and copy it into /system and /system/bin

IMPORTANT:
Find tiwlan0 and rename it into wlan0

Take META-INF folder from shakira folder and edit updater-script if needed.
Zip the package and flash.
