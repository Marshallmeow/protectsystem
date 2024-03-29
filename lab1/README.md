---
title: "First practice"
format: md
author: "Yakovlev Alex"
date: "06.03.2023"
editor: visual
---

## Получение сведений о системе

## Цель работы

Получить сведения об используемой системе

## Ход работы

1.  Получение сведений о версии ядра:

    ```{bash}
    uname -r
    ```

<div>

    5.10.0-9-amd64

</div>

2.  Получение всех сведений о ядре:

    ```{bash}
    uname -a
    ```

    <div>

        Linux debian11 5.10.0-21-amd64 #1 SMP Debian 5.10.162-1 (2023-01-21) x86_64 GNU/Linux

    </div>

3.  Получение сведений об используемом дистрибутиве:

    ```{bash}
    sudo lsb_release -a
    ```

    <div>

        Distributor ID: Debian
        Description:    Debian GNU/Linux 11 (bullseye)
        Release:    11
        Codename:   bullseye

    </div>

4.  Получение данных о модели процессора:

    ```{bash}
    cat /proc/cpuinfo | grep "model name"
    ```

    <div>

        model name  : Intel(R) Core(TM) i7-10750H CPU @ 2.60GHz
        model name  : Intel(R) Core(TM) i7-10750H CPU @ 2.60GHz

    </div>

5.  Получение последних 30 строк системных логов:

    ```{bash}
    sudo dmesg | tail -n 30
    ```

<div>

    [    2.863620] EXT4-fs (dm-4): mounted filesystem with ordered data mode. Opts: (null)
    [    2.872607] systemd-journald[241]: Received client request to flush runtime journal.
    [    2.932503] audit: type=1400 audit(1678097920.396:2): apparmor="STATUS" operation="profile_load" profile="unconfined" name="lsb_release" pid=457 comm="apparmor_parser"
    [    2.938912] audit: type=1400 audit(1678097920.404:3): apparmor="STATUS" operation="profile_load" profile="unconfined" name="nvidia_modprobe" pid=470 comm="apparmor_parser"
    [    2.938915] audit: type=1400 audit(1678097920.404:4): apparmor="STATUS" operation="profile_load" profile="unconfined" name="nvidia_modprobe//kmod" pid=470 comm="apparmor_parser"
    [    2.958028] audit: type=1400 audit(1678097920.424:5): apparmor="STATUS" operation="profile_load" profile="unconfined" name="libreoffice-xpdfimport" pid=471 comm="apparmor_parser"
    [    2.987679] audit: type=1400 audit(1678097920.452:6): apparmor="STATUS" operation="profile_load" profile="unconfined" name="libreoffice-senddoc" pid=473 comm="apparmor_parser"
    [    3.020338] snd_intel8x0 0000:00:05.0: allow list rate for 1028:0177 is 48000
    [    3.079062] audit: type=1400 audit(1678097920.512:7): apparmor="STATUS" operation="profile_load" profile="unconfined" name="libreoffice-soffice" pid=456 comm="apparmor_parser"
    [    3.079065] audit: type=1400 audit(1678097920.512:8): apparmor="STATUS" operation="profile_load" profile="unconfined" name="libreoffice-soffice//gpg" pid=456 comm="apparmor_parser"
    [    3.079471] audit: type=1400 audit(1678097920.544:9): apparmor="STATUS" operation="profile_load" profile="unconfined" name="/usr/bin/evince" pid=475 comm="apparmor_parser"
    [    3.079473] audit: type=1400 audit(1678097920.544:10): apparmor="STATUS" operation="profile_load" profile="unconfined" name="/usr/bin/evince//sanitized_helper" pid=475 comm="apparmor_parser"
    [    3.625823] e1000: enp0s3 NIC Link is Up 1000 Mbps Full Duplex, Flow Control: RX
    [    3.626175] IPv6: ADDRCONF(NETDEV_CHANGE): enp0s3: link becomes ready
    [    6.937544] vboxvideo: loading version 6.1.28 r147628
    [    6.977425] 10:18:44.443746 main     VBoxService 6.1.28 r147628 (verbosity: 0) linux.amd64 (Oct 18 2021 20:11:04) release log
                   10:18:44.443748 main     Log opened 2023-03-06T10:18:44.443743000Z
    [    6.977463] 10:18:44.443809 main     OS Product: Linux
    [    6.977486] 10:18:44.443839 main     OS Release: 5.10.0-21-amd64
    [    6.977505] 10:18:44.443861 main     OS Version: #1 SMP Debian 5.10.162-1 (2023-01-21)
    [    6.977530] 10:18:44.443879 main     Executable: /opt/VBoxGuestAdditions-6.1.28/sbin/VBoxService
                   10:18:44.443880 main     Process ID: 705
                   10:18:44.443880 main     Package type: LINUX_64BITS_GENERIC
    [    6.978525] 10:18:44.444873 main     6.1.28 r147628 started. Verbose level = 0
    [    6.979919] 10:18:44.446248 main     vbglR3GuestCtrlDetectPeekGetCancelSupport: Supported (#1)
    [    9.483417] rfkill: input handler disabled
    [   13.424992] rfkill: input handler enabled
    [   15.640842] rfkill: input handler disabled
    [   15.729557] process 'VBoxClient' launched '/opt/VBoxGuestAdditions-6.1.28/bin/VBoxDRMClient' with NULL argv: empty string added
    [  192.610152] TCP: request_sock_TCP: Possible SYN flooding on port 5148. Sending cookies.  Check SNMP counters.

</div>

## Вывод

Таким образом, было проведено ознакомление с базовыми командами ОС Linux\\Debian 11 и интерфейсом программной среды r-studio.
