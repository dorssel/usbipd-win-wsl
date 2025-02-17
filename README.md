<!--
SPDX-FileCopyrightText: 2025 Frans van Dorsselaer

SPDX-License-Identifier: GPL-3.0-only
-->

# usbipd-win-wsl

This is a helper project to build a distribution independent `usbip` client for Windows Subsystem for Linux (WSL).
The binaries are used in the main project [usbipd-win](https://github.com/dorssel/usbipd-win).

The binary `usbip` is built from sources subject to different (compatible) licenses:

- Part of the Linux kernel, in particular the sources in `tools/usb/usbip`

  Note that the subset of sources in `tools/usb/usbip` are licensed under GNU General Public License, version 2 *or later*.

- `libudev-zero`

  `usbip` is statically linked against `libudev-zero` subject to the terms and conditions of the
  [ISC License](https://opensource.org/license/isc-license-txt/).
