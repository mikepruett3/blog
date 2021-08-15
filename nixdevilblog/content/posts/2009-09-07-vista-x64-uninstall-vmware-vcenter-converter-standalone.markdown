---
title: "Vista x64 Uninstall VMware vCenter Converter Standalone"
slug: vista-x64-uninstall-vmware-vcenter-converter-standalone
date: 2009-09-07 22:16:32+00:00
author: "Mike Pruett"
draft: false
layout: post
comments: true
tags: [vmware,windows]
categories: [Homelab]
---

If you are using Vista x64 and are trying to uninstall VMware vCenter Converter Standalone like I was, you may run into the following issue uninstalling...

```log
Error 1321. The Installer has insufficient privileges to modify the file
C:\ProgramData\VMware\VMWare vCenter Converter Standalone\ssl\rui.key
```

This aparently is due to a permissions issue on the following file:

```log
C:\ProgramData\VMware\VMWare vCenter Converter Standalone\ssl\rui.key
```

The minute you give yourself permissions to that file, you then can successfully uninstall it. Yay!!

Thanks to those guys at the [VMTN forums](http://communities.vmware.com/message/1344322)! You guys rock!!
