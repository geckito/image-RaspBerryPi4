Minimalistic Raspberry Pi4
==========================

This image is based on the JeOS image, but further reduced.

You will *not* be able to update or install further packages using 
zypper in the running system. Tthere is also no YaST to configure 
things.

This image description is supposed to get adapted and the image
rebuild for modifications instead.

Ideally we will have just the kernel and busybox running
here, but we are not there yet.

Build
=====

Build it using pbuild with following parameters:

Install pbuild via package or via git:


```shell
# git clone https://github.com/openSUSE/obs-build.git SOMEHWERE
# SOMWHERE/pbuild --vm-type=kvm --vm-memory=4096 --vm-disk-size=6144
```

Todo
====

* fix vc4 initialisation

* delete more packages / reduce size further (currently still above 400MB)

* make it easy to boot into a shell or own executables
  instead of providing a login prompt.

* document how to setup network as user

