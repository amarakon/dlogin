Dlogin – dmenu Login
================

## Contents

-   [Usage](#usage)
-   [Dependencies](#dependencies)
-   [Dependencies](#dependencies-1)
-   [Installation](#installation)
    -   [Universal](#universal)
    -   [Gentoo](#gentoo)
-   [Uninstallation](#uninstallation)
    -   [Universal](#universal-1)
    -   [Gentoo](#gentoo-1)

Dlogin is a simple program to manage login via dmenu. It supports on any
init system and it works regardless if you have polkit installed.

## Usage

``` sh
`# user` dlogin # run the program
```

## Dependencies

1.  dmenu
2.  [doas\_askpass](https://github.com/amarakon/doas_askpass) (if you do
    not have polkit installed)

## Dependencies

1.  dmenu
2.  xclip (if you want to use the *copy* or *copy file* features.)

## Installation

### Universal

``` sh
`# user` git clone https://github.com/amarakon/dlogin
`# user` cd dlogin
`# root` make install
```

### Gentoo

``` sh
`# root` eselect repository add amarlay git https://github.com/amarakon/amarlay
`# root` emerge --sync amarlay
`# root` emerge x11-misc/dlogin
```

## Uninstallation

### Universal

``` sh
`# user` cd dlogin
`# root` make uninstall
```

### Gentoo

``` sh
`# root` emerge -c x11-misc/dlogin
# Remove my overlay (optional)
`# root` eselect-repository remove -f amarlay
`# root` emerge --sync
```
