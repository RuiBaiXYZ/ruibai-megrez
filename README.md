# ruibai-megrez
The RuiBai Megrez Project's unique mission is to build a free and opensource tool for making diagrams and GUI prototyping that everyone can use. Forked from https://github.com/evolus/pencil started at 2022-06-17

## Compile

### RockyLinux 8.5

https://www.electronjs.org/docs/latest/development/build-instructions-linux

dnf install clang dbus-devel gtk3-devel libnotify-devel libgnome-keyring-devel xorg-x11-server-utils libcap-devel cups-devel libXtst-devel alsa-lib-devel libXrandr-devel nss-devel python-dbusmock

#### dependencies
dnf -y install GConf2 GConf2-devel


### build
rm -Rf node_modules/ package-lock.json && npm install && npm run postinstall && npm run dist:linux
