sane-overlay
============

A gentoo overlay containing updated sane-backends.

Installing
----------

Using eselect repository:
```
eselect repository add sane-overlay git https://github.com/brulzki/sane-overlay.git
```

Using layman:
```
layman -o https://raw.github.com/brulzki/sane-overlay/master/repository.xml -f -a sane-overlay
```

### Manual install

Add the following file at /etc/portage/repos.conf/sane-overlay.conf

```
[sane-overlay]
location = /var/db/repos/sane-overlay
sync-uri = https://github.com/brulzki/sane-overlay.git
sync-type = git
clone-depth = 0
```

Then run this command to download the overlay:

```
emaint sync -r sane-overlay
```

live ebuild
-----------

Install the latest git development version

```
ACCEPT_KEYWORDS="**" emerge -1 =media-gfx/sane-backends-9999
```
