sane-overlay
============

A gentoo overlay containing updated sane-backends.

Installing
----------

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
