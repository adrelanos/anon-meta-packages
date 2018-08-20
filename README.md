# Recommended packages for VMs other than Qubes VMs #

A metapackage, which includes recommended packages which are useful within
non-Qubes virtual machines. These are not useful in Qubes, since Qubes already
has native implementations for those.

Safe to remove, if you know what you are doing.

Package: anon-shared-packages-dependencies
Architecture: all
Depends: bzip2, file, lsof, most, pciutils, strace, sysfsutils,
less, haveged, locales, apt-transport-https, apt-transport-tor,
sdwdate, bootclockrandomization, timesanitycheck,
timezone-utc, vbox-disable-timesync, busybox,
security-misc, ${misc:Depends}
Description: Dependencies for both, Anon-Gateway and Anon-Workstation CLI
# Dependencies for both, Anon-Gateway and Anon-Workstation CLI #

A metapackage, which installs command line interface (CLI) packages which
both, Anon-Gateway and Anon-Workstation, depend on.

Do not remove.

Package: anon-shared-packages-recommended
Architecture: all
Depends: bash-completion, command-not-found, zsh, nano, wget, dnsutils,
iputils-ping, apparmor-utils,
apparmor-profile-anondist, udisks2, secure-delete, sudo, net-tools,
gpl-sources-download,
scurl, security-misc, tor-ctrl, uwt, openvpn, ntfs-3g,
usability-misc, menu, man-db, anon-apps-config, open-link-confirmation,
${misc:Depends}
Description: Recommended packages for both, Anon-Gateway and Anon-Workstation CLI
# Recommended packages for both, Anon-Gateway and Anon-Workstation CLI #

A metapackage, which includes recommended packages to ensure, Debian GNU/Linux
standard tools are available and other useful recommended packages for a
command line interface (CLI) based Anon-Gateway or Anon-Workstation.

Safe to remove, if you know what you are doing.

Package: anon-shared-default-applications
Architecture: all
Pre-Depends: whonix-legacy
Depends: sdwdate-gui, msgcollector-gui, anon-iceweasel-warning, anon-icon-pack,
${misc:Depends}
Description: Recommended desktop packages for both, Anon-Gateway and Anon-Workstation GUI
# Recommended desktop packages for both, Anon-Gateway and Anon-Workstation GUI #

A metapackage, which installs recommended graphical user interface (GUI)
default applications, which are useful in a default installation of a
Tor-Gateway or Tor-Workstation desktop.

Safe to remove, if you know what you are doing.

Package: anon-gateway-packages-dependencies
Architecture: all
Pre-Depends: whonix-legacy
Depends: tor, anon-gw-base-files, ipv4-forward-disable,
ipv6-disable, ${misc:Depends}
Description: Dependencies for Anon-Gateway CLI
# Dependencies for Anon-Gateway CLI #

A metapackage, which installs command line interface (CLI) packages
which Anon-Gateway depends on.

Do not remove.

Package: anon-gateway-packages-recommended
Architecture: all
Pre-Depends: whonix-legacy
Depends: tor-geoipdb, tor-arm, obfsproxy, obfs4proxy, flashproxy-client,
fteproxy, onion-grater, ${misc:Depends}
Description: Recommended packages for Anon-Gateway CLI
# Recommended packages for Anon-Gateway CLI #

A metapackage, which installs packages, which are recommended for
a command line interface (CLI) based Tor-Gateway.

Safe to remove, if you know what you are doing.

Package: anon-gateway-default-applications
Architecture: all
Pre-Depends: whonix-legacy
Depends: onioncircuits, anon-connection-wizard, tor-control-panel,
${misc:Depends}
Description: Recommended desktop packages for Anon-Gateway GUI
# Recommended desktop packages for Anon-Gateway GUI #

A metapackage, which installs graphical user interface (GUI) packages,
which are recommended for a graphical Tor-Gateway.

Safe to remove, if you know what you are doing.

Package: anon-workstation-packages-dependencies
Architecture: all
Pre-Depends: whonix-legacy
Depends: anon-ws-base-files, ${misc:Depends}
Recommends: anon-workstation-packages-recommended
Description: Dependencies for Anon-Workstation CLI
# Dependencies for Anon-Workstation CLI #

A metapackage, which installs command line interface (CLI) packages which
Anon-Workstation depends on.

Do not remove.

Package: anon-workstation-packages-recommended
Architecture: all
Pre-Depends: whonix-legacy
Depends: xchat-improved-privacy, anon-mixmaster, anon-gpg-tweaks, anon-torchat,
anon-ws-disable-stacked-tor, youtube-dl,
thunderbird, enigmail, xul-ext-torbirdy, pwgen,
python-msgpack, bindp, codecrypt, gnupg2, gnupg-agent, dirmngr,
${misc:Depends}
Description: Recommended packages for Anon-Workstation
# Recommended packages for Anon-Workstation #

A metapackage, which installs packages, which are recommended for
Anon-Workstation, because they are useful for a Tor Workstation.

Feel free to remove if you know what you are doing.

Package: anon-shared-desktop
Architecture: all
Depends: xserver-xorg, xserver-xorg-video-qxl, xserver-xorg-video-fbdev,
xserver-xorg-video-vesa, libgl1-mesa-dri, upower, gtk2-engines-pixbuf,
${misc:Depends}
Description: Desktop Depends
# Desktop Depends #

A metapackage, which installs dependencies for desktop environments,
such as KDE, GNOME, etc.

anon-shared-desktop-kde depends on this package.

Package: anon-shared-desktop-kde
Architecture: all
Depends: anon-shared-desktop, sddm, kde-config-sddm,
plasma-desktop, plasma-desktop-data, kwin-x11, ${misc:Depends}
Description: Recommended packages for Gateway/Workstation base KDE desktop
# Recommended packages for Gateway/Workstation base KDE desktop #

A metapackage, which installs a minimal, yet complete enough
to contain the very basics, KDE desktop. The Anon-Gateway desktop and the
Anon-Workstation desktop depend on this package.

Safe to remove.

Package: anon-shared-applications-kde
Architecture: all
Depends: kdesudo, kscreen, polkit-kde-agent-1, kdepasswd, kfind,
ksysguard, konsole, kwrite, dolphin, baloo-kf5, ark, systemsettings,
p7zip-full, zip, unzip, ksystemlog, gtk2-engines-oxygen,
gtk3-engines-breeze, plasma-pa,
kde-config-gtk-style, kde-config-gtk-style-preview,
kde-config-screenlocker, kde-config-sddm, kde-style-oxygen-qt5,
kmenuedit, ${misc:Depends}
Description: Recommended applications for Gateway/Workstation KDE desktop
# Recommended applications for Gateway/Workstation KDE desktop #

A metapackage, which installs a minimal, yet complete enough
to contain the very basics, KDE applications.

Safe to remove.

Package: anon-shared-kde-accessibility
Architecture: all
Depends: gnome-orca,
console-braille, florence, dasher, kdeaccessibility, kvkbd, kmousetool, kmag,
kmouth, jovie, xbrlapi, festival, qt-at-spi, ${misc:Depends}
Description: KDE accessibility tools
# KDE accessibility tools #

A metapackage, which installs accessibility tools for the KDE desktop.

Safe to remove, if you know what you are doing.

Package: anon-workstation-default-applications
Architecture: all
Depends: hexchat, vlc, mixmaster, kcalc, okular,
gwenview, libkf5kipi31.0.0, libkf5kipi-data,
kgpg, mat, python-hachoir-core, python-hachoir-parser,
python-pdfrw, python-cairo, python-poppler, python-mutagen,
libimage-exiftool-perl, gir1.2-gtk-3.0,
pinentry-qt | pinentry-x11,
tb-default-browser, tb-starter, tb-updater, youtube-dl,
thunderbird, enigmail, xul-ext-torbirdy, ricochet-im, coyim,
${misc:Depends}
Description: Recommended default applications for a graphical Anon-Workstation GUI
# Recommended default applications for a graphical Anon-Workstation GUI #

A metapackage, which installs recommended GUI default applications,
which are useful in a default installation of a graphical Tor Workstation.

Safe to remove, if you know what you are doing.

Package: anon-workstation-extra-applications
Architecture: all
Depends: ${misc:Depends}
Recommends: anon-workstation-packages-recommended,
anon-workstation-default-applications, shutter,
gtk-recordmydesktop, libreoffice, kdenlive, kolourpaint4
Description: Complements anon-workstation-default-applications
# Complements anon-workstation-default-applications #

A metapackage, which installs extra applications, to complement the
default applications.

Does not get installed by default, because extra applications
take too much space and are not required for everyone.

Package: anon-workstation-langpack-common
Architecture: all
Depends: ${misc:Depends}
Recommends: iceweasel-l10n-all | firefox-l10n-all, ttf-dejavu, ttf-liberation, locales-all,
ttf-kacst, ttf-farsiweb, scim-pinyin, scim-tables-zh, scim-uim, ttf-arphic-ukai, ttf-arphic-uming,
culmus, libfribidi0, ttf-indic-fonts, scim-anthy, ttf-khmeros, ttf-unfonts-core, ttf-lao,
ttf-thai-tlwg, xfonts-intl-chinese, xfonts-wqy, xfonts-bolkhov-koi8r-75dpi,
xfonts-bolkhov-koi8r-misc, xfonts-cronyx-koi8r-100dpi
Description: Fonts and language packages for better internationalization support
# Fonts and language packages for better internationalization support #

A metapackage which installs fonts and language packages for better
internationalization support.

Does not get installed by default, because it is largely untested
and needs more work.

Package: anon-shared-desktop-langpack-kde
Architecture: all
Depends: ${misc:Depends}
Recommends: kde-l10n-ar, kde-l10n-bg, kde-l10n-bs,
kde-l10n-ca, kde-l10n-cavalencia, kde-l10n-cs, kde-l10n-da, kde-l10n-de, kde-l10n-el, kde-l10n-engb,
kde-l10n-es, kde-l10n-et, kde-l10n-eu, kde-l10n-fa, kde-l10n-fi, kde-l10n-fr, kde-l10n-ga,
kde-l10n-gl, kde-l10n-he, kde-l10n-hr, kde-l10n-hu, kde-l10n-ia, kde-l10n-id, kde-l10n-is,
kde-l10n-it, kde-l10n-ja, kde-l10n-kk, kde-l10n-km, kde-l10n-ko, kde-l10n-lt, kde-l10n-lv,
kde-l10n-nb, kde-l10n-nds, kde-l10n-nl, kde-l10n-nn, kde-l10n-pa, kde-l10n-pl, kde-l10n-pt,
kde-l10n-ptbr, kde-l10n-ro, kde-l10n-ru, kde-l10n-si, kde-l10n-sk, kde-l10n-sl, kde-l10n-sr,
kde-l10n-sv, kde-l10n-tg, kde-l10n-th, kde-l10n-tr, kde-l10n-ug, kde-l10n-uk, kde-l10n-vi,
kde-l10n-wa, kde-l10n-zhcn, kde-l10n-zhtw, anon-workstation-langpack-common
Description: Extra language support for the KDE desktop
# Extra language support for the KDE desktop #

A metapackage, which includes extra language support for the
KDE desktop.

Does not get installed by default, because it takes a lot of
space and requires a better solution.

Package: apparmor-profiles-whonix
Architecture: all
Depends: apparmor-profile-icedove,
apparmor-profile-torbrowser,
apparmor-profile-xchat,
apparmor-profile-gwenview, apparmor-profile-okular, ${misc:Depends}
Description: Extra AppArmor profiles developed by the Whonix team
# Extra AppArmor profiles developed by the Whonix team #

A metapackage, which installs apparmor profiles developed by the Whonix team.

Increases security.

Safe to remove, if you know what you are doing.

Package: whonix-gateway-packages-dependencies-pre
Architecture: all
Depends: whonix-gw-network-conf, anon-base-files,
${misc:Depends}
Description: Dependencies for Whonix-Gateway that changes network related files
# Dependencies for Whonix-Gateway that changes network related files #

A metapackage, which installs packages which Whonix-Gateway
depends on. Can not be merged into whonix-gateway-packages-dependencies due to
conflicts with chroot build process.

Do not remove.

Package: whonix-gateway-packages-dependencies
Architecture: all
Pre-Depends: whonix-legacy
Depends: anon-gateway-packages-dependencies, anon-gw-anonymizer-config,
whonix-gateway-packages-dependencies-pre, ${misc:Depends}
Description: Dependencies for Whonix-Gateway
# Dependencies for Whonix-Gateway #

A metapackage, which installs packages which Whonix-Gateway
depends on.

Do not remove.

Package: whonix-gateway-packages-recommended
Architecture: all
Pre-Depends: whonix-legacy
Depends: whonix-gw-desktop-shortcuts, whonix-gw-kde-desktop-conf,
whonixsetup, whonix-setup-wizard, ${misc:Depends}
Recommends: anon-gateway-packages-recommended
Description: Recommended packages for Whonix-Gateway
# Recommended packages for Whonix-Gateway #

A metapackage, which installs packages, which are recommended for
Whonix-Gateway.

Safe to remove, if you know what you are doing.

Package: whonix-shared-packages-dependencies
Architecture: all
Pre-Depends: whonix-legacy
Depends: whonix-base-files, anon-apt-sources-list, whonix-firewall,
whonix-initializer, whonix-repository, grub-enable-apparmor,
${misc:Depends}
Description: Dependencies for Whonix-Gateway and Whonix-Workstation
# Dependencies for Whonix-Gateway and Whonix-Workstation #

A metapackage, which installs packages which both, Whonix-Gateway
and Whonix-Workstation, depend on.

Do not remove.

Package: whonix-shared-packages-recommended
Architecture: all
Depends: anon-shared-packages-recommended, whonixcheck,
${misc:Depends}
Description: Recommended packages for Whonix-Gateway and Whonix-Workstation
# Recommended packages for Whonix-Gateway and Whonix-Workstation #

A metapackage, which includes recommended packages to ensure, Whonix
standard tools are available and other useful recommended packages.

Safe to remove, if you know what you are doing.

Package: whonix-workstation-packages-dependencies-pre
Architecture: all
Depends: whonix-ws-network-conf, anon-ws-dns-conf, anon-base-files,
${misc:Depends}
Description: Dependencies for Whonix-Workstation that changes network related files
# Dependencies for Whonix-Workstation that changes network related files #

A metapackage, which installs packages which Whonix-Workstation
depends on. Can not be merged into whonix-workstation-packages-dependencies
due to conflicts with chroot build process.

Do not remove.

Package: whonix-workstation-packages-dependencies
Architecture: all
Pre-Depends: whonix-legacy
Depends: whonix-workstation-packages-dependencies-pre,
${misc:Depends}
Recommends: whonix-workstation-packages-recommended
Description: Dependencies for Whonix-Workstation
# Dependencies for Whonix-Workstation #

A metapackage, which installs packages which Whonix-Workstation
depends on.

Do not remove.

Package: whonix-workstation-packages-recommended
Architecture: all
Depends: whonix-ws-desktop-shortcuts, whonix-ws-irc-chat-support,
whonix-welcome-page, whonix-ws-start-menu-additions,
${misc:Depends}
Recommends: anon-workstation-packages-recommended
Description: Recommended packages for Whonix-Workstation CLI
# Recommended packages for Whonix-Workstation CLI #

A metapackage, which installs packages, which are recommended for
command line interface (CLI) Whonix-Workstation, because they are
useful for a Tor Workstation.

Feel free to remove if you know what you are doing.

Package: whonix-gateway-shared-packages-shared-meta
Architecture: all
Pre-Depends: whonix-legacy
Depends: whonix-gateway-packages-dependencies-pre,
anon-shared-packages-dependencies,
anon-shared-packages-recommended,
anon-shared-applications-kde,
anon-shared-default-applications,
whonix-shared-packages-dependencies,
whonix-shared-packages-recommended,
anon-gateway-packages-dependencies,
anon-gateway-packages-recommended,
anon-gateway-default-applications,
whonix-gateway-packages-dependencies,
whonix-gateway-packages-recommended,
${misc:Depends}
Description: Whonix-Gateway Shared Packages
# Whonix-Gateway Shared Packages #

A metapackage, which installs packages, for a Whonix-Default-Gateway.

It is shared between Qubes-Whonix and Non-Qubes-Whonix.

It will install build chroot scripts, but not run them.

Feel free to remove if you know what you are doing.

Package: whonix-workstation-shared-packages-shared-meta
Architecture: all
Pre-Depends: whonix-legacy
Depends: whonix-workstation-packages-dependencies-pre,
anon-shared-packages-dependencies,
anon-shared-packages-recommended,
anon-shared-applications-kde,
anon-shared-default-applications,
whonix-shared-packages-dependencies,
whonix-shared-packages-recommended,
anon-workstation-packages-dependencies,
anon-workstation-packages-recommended,
anon-workstation-default-applications,
whonix-workstation-packages-dependencies,
whonix-workstation-packages-recommended,
${misc:Depends}
Description: Whonix-Workstation Shared Packages
# Whonix-Workstation Shared Packages #

A metapackage, which installs packages, for a Whonix-Default-Workstation.

It is shared between Qubes-Whonix and Non-Qubes-Whonix.

It will install build chroot scripts, but not run them.

Feel free to remove if you know what you are doing.

Package: qubes-whonix-gateway
Architecture: all
Depends: whonix-gateway-shared-packages-shared-meta, qubes-whonix,
qubes-whonix-shared-packages-recommended,
qubes-whonix-gateway-packages-recommended, ${misc:Depends}
Replaces: whonix-gateway
Description: Default packages for Qubes-Whonix-Gateway
# Default packages for Qubes-Whonix-Gateway #

A metapackage, which installs packages, for a
Qubes-Whonix-Default-Gateway.

Only depends on whonix-gateway-shared-packages-shared-meta,
because installing anon-shared-desktop is not required in
Qubes-Whonix.

Feel free to remove if you know what you are doing.

Package: qubes-whonix-workstation
Architecture: all
Depends: whonix-workstation-shared-packages-shared-meta, qubes-whonix,
qubes-whonix-shared-packages-recommended,
qubes-whonix-workstation-packages-recommended, ${misc:Depends}
Replaces: whonix-workstation
Description: Default Packages for Qubes-Whonix-Workstation
# Default Packages for Qubes-Whonix-Workstation #

A metapackage, which installs packages, for a
Qubes-Whonix-Default-Workstation.

Only depends on whonix-workstation-shared-packages-shared-meta,
because installing anon-shared-desktop is not required in
Qubes-Whonix.

Feel free to remove if you know what you are doing.

Package: non-qubes-whonix-gateway
Architecture: all
Depends: whonix-gateway-shared-packages-shared-meta, non-qubes-vm-enhancements,
anon-shared-desktop, anon-shared-desktop-kde,
${misc:Depends}
Replaces: whonix-gateway
Description: Default Packages for Non-Qubes-Whonix-Gateway
# Default Packages for Non-Qubes-Whonix-Gateway #

A metapackage, which installs packages, for a
Non-Qubes-Whonix-Default-Gateway.

Depends on whonix-gateway-shared-packages-shared-meta,
and anon-shared-desktop because that is required in
Non-Qubes-Whonix in order to get graphical desktop environment.

Feel free to remove if you know what you are doing.

Package: non-qubes-whonix-workstation
Architecture: all
Depends: whonix-workstation-shared-packages-shared-meta, non-qubes-vm-enhancements,
anon-shared-desktop, anon-shared-desktop-kde,
${misc:Depends}
Replaces: whonix-workstation
Description: Default Packages for Non-Qubes-Whonix-Workstation
# Default Packages for Non-Qubes-Whonix-Workstation #

A metapackage, which installs packages, for a
Non-Qubes-Whonix-Default-Workstation.

Depends on whonix-workstation-shared-packages-shared-meta,
and anon-shared-desktop because that is required in
Non-Qubes-Whonix in order to get graphical desktop environment.

Feel free to remove if you know what you are doing.
## How to install `anon-meta-packages` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org stretch main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-meta-packages`.

```
sudo apt-get install anon-meta-packages
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `anon-meta-packages` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`anon-meta-packages` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
