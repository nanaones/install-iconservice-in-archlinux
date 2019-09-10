# How to install iconservice in Archlinux


Write this guide for this [discuss](https://www.icondev.io/discuss/5d76c519fe6149005a3d6104)




# Install

`$ sudo pacman -Syu`

`$ sudo pacman -S libsecp256k1 python-pip pkg-config gcc`

`$ pip3 install iconservice`




# Steps

First of all, update pacman using 'sudo' command

`$ sudo pacman -Syu`

Then, install libsecp256k1  

`$ pacman -S libsecp256k1`


```
[root@b500b8171487 home]# pacman -S libsecp256k1
resolving dependencies...
looking for conflicting packages...

Packages (1) libsecp256k1-20190822+995+ge729cc7-1

Total Download Size:   0.11 MiB
Total Installed Size:  0.20 MiB

:: Proceed with installation? [Y/n] y
:: Retrieving packages...
 libsecp256k1-20190822+995+ge729cc7-1-x86_64            110.5 KiB  99.5K/s 00:01 [##############################################] 100%(1/1) checking keys in keyring                                                   [##############################################] 100%(1/1) checking package integrity

 ...

```
---

install python3 and pip

`$ pacman -S python`

`$ pacman -S python-pip`


```
[root@b500b8171487 home]# pacman -S python
resolving dependencies...
looking for conflicting packages...

Packages (2) libnsl-1.2.0-1  python-3.7.4-1

Total Download Size:    33.99 MiB
Total Installed Size:  144.66 MiB

:: Proceed with installation? [Y/n] y
:: Retrieving packages...
 libnsl-1.2.0-1-x86_64                                   57.3 KiB   110K/s 00:01 [##############################################] 100% python-3.7.4-1-x86_64                                   33.9 MiB  1398K/s 00:25 [##############################################] 100%

 ...


```


```

[root@b500b8171487 home]# pacman -S python-pip
resolving dependencies...
looking for conflicting packages...

Packages (26) python-appdirs-1.4.3-2  python-attrs-19.1.0-1  python-cachecontrol-0.12.5-4  python-chardet-3.0.4-2
              python-colorama-0.4.1-1  python-distlib-0.2.9-1  python-distro-1.4.0-1  python-html5lib-1.0.1-3  python-idna-2.8-1
              python-importlib-metadata-0.20-1  python-lockfile-0.12.2-4  python-more-itertools-4.3.0-2  python-msgpack-0.6.1-1
              python-packaging-19.1-2  python-pep517-0.6.0-1  python-progress-1.5-1  python-pyparsing-2.4.2-1  python-pytoml-0.1.21-1
              python-requests-2.22.0-1  python-retrying-1.3.3-4  python-setuptools-1:41.2.0-1  python-six-1.12.0-1
              python-urllib3-1.25.3-1  python-webencodings-0.5.1-2  python-zipp-0.6.0-1  python-pip-19.0.3-1

Total Download Size:    2.02 MiB
Total Installed Size:  10.93 MiB

:: Proceed with installation? [Y/n] y
:: Retrieving packages...
 python-appdirs-1.4.3-2-any                              14.2 KiB  1416K/s 00:00 [##############################################] 100% python-attrs-19.1.0-1-any                               51.1 KiB   150K/s 00:00 [##############################################] 100% python-pyparsing-2.4.2-1-any                           104.5 KiB   124K/s 00:01 [##############################################] 100%

 ...

```
---

### install pkg-config

`$ sudo pacman -S pkg-config`

```
[root@b500b8171487 home]# pacman -S pkg-config
resolving dependencies...
looking for conflicting packages...

Packages (1) pkgconf-1.6.3-2

Total Download Size:   0.05 MiB
Total Installed Size:  0.23 MiB

:: Proceed with installation? [Y/n] y
:: Retrieving packages...
 pkgconf-1.6.3-2-x86_64                                  54.7 KiB   130K/s 00:00 [##############################################] 100%(1/1) checking keys in keyring                                                   [##############################################] 100%(1/1) checking package integrity                                                 [##############################################] 100%(1/1) loading package files                                                      [##############################################] 100%(1/1) checking for file conflicts                                                [##############################################] 100%(1/1) checking available disk space                                              [##############################################] 100%:: Processing package changes...
(1/1) installing pkgconf                                                         [##############################################] 100%:: Running post-transaction hooks...
(1/2) Arming ConditionNeedsUpdate...

...

```

---
### install gcc 
`$ sudo pacman -S gcc`



```

[root@b500b8171487 home]# pacman -S gcc
resolving dependencies...
looking for conflicting packages...

Packages (4) binutils-2.32-2  libmpc-1.1.0-1  mpfr-4.0.2-1  gcc-9.1.0-2

Total Download Size:    39.14 MiB
Total Installed Size:  170.72 MiB

:: Proceed with installation? [Y/n] y
:: Retrieving packages...
 binutils-2.32-2-x86_64                                   4.8 MiB   958K/s 00:05 [##############################################] 100% mpfr-4.0.2-1-x86_64                                    313.8 KiB   165K/s 00:02 [##############################################] 100% libmpc-1.1.0-1-x86_64                                   64.7 KiB   127K/s 00:01 [##############################################] 100% gcc-9.1.0-2-x86_64                                      33.9 MiB  1245K/s 00:28 [##############################################] 100%(4/4) checking keys in keyring                                                   [##############################################] 100%

...

```

---

### Finally, install iconservice 

`$ pip3 install iconservice`

```
[root@b500b8171487 home]# pip3 install iconservice
Collecting iconservice
  Using cached https://files.pythonhosted.org/packages/b5/13/acf09186570dc30b807d45acfd6733b3c6ee97c29838fb751383948b8d27/iconservice-1.4.3-py3-none-any.whl
Requirement already satisfied: plyvel>=1.0.5 in /usr/lib/python3.7/site-packages (from iconservice) (1.1.0)
...


```

---

### import check

```
[root@b500b8171487 home]# python3
Python 3.7.4 (default, Jul 16 2019, 07:12:58)
[GCC 9.1.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import iconservice
>>> exit()

```

