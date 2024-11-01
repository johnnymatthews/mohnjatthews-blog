---
title: "Install Vagrant on Windows 11"
description: "Vagrant is a useful tool for spinning up local virtual machines, but getting it to run properly on Windows 11 can be a pain. This guide quickly runs through installing it, and spinning up a VM."
date: 2024-11-01
---

## Prerequisites

There are a couple of things we need to install before we can start spinning up VMs:

- Vagrant
- VirtualBox

1. The first step is to install Vagrant. This process is super simple if you just use [winget](https://learn.microsoft.com/en-us/windows/package-manager/winget/), which is essentially Microsoft's package manager:

    ```shell
    winget install vagrant
    ```

1. Next, we'll install VirtualBox. Vagrant requires a _host_ virtual machine manager, and VirtualBox is free and easy to use, so we're gonna use that one:

    ```shell
    winget install Oracle.VirtualBox -v 7.0.6
    ```

    A quick note here: the maintainers of Vagrant are pretty slow when it comes to updating their software. At the time of writing, Vagrant only supports VirtualBox up to version 7.0.6, while the latest VirtualBox release is at 7.1.4. I'm assuming that the maintainers of Vagrant will update their stuff to support the latest VirtualBox release. Still, for now, we're stuck specifying which version we want when calling Winget.

1. Once both Vagrant and VirtualBox are installed, you'll need to grab the **VirtualBox Extension Pack** from [virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads).
1. Open VirtualBox, click **File**, **Tools**, **Extension Pack Manager**.
1. Click **Install** and select the `Oracle_VirtualBox_Extension_Pack.vbox-extpack` file you just downloaded. VirtualBox takes about 2 minutes to install the pack.

## Running a VM

We have to follow a few steps to get a VM up and running.

1. Add the VirtualBox installation location to your current `$PATH` variable:

    ```shell
    $env:Path += ";C:\Program Files\Oracle\VirtualBox\"
    ```

    You _can_ add this globally, so you don't have to run this every time, but that requires dealing with a GUI and/or the registry. I just can't be bothered doing that.

1. Create a `Vagrantfile`. If you're familiar with Vagrant, then I'm assuming you already know what a `Vagrantfile` is. If you _don't_, go check out the [Vagrant docs](https://developer.hashicorp.com/vagrant/intro).
1. Spin up the VM using `vagrant up`:

    ```shell
    vagrant up --provider=virtualbox
    ```

    For some reason, I always need to add the `--provider` tag to tell Vagrant exactly which provider I'm using. It might just be my setup, though.

## Done

And that's about it! All in all, it's not too complicated. There are just some steps that might not be completely obvious.
