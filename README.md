# ddrescue 2.4

A ddrescue static binary that runs on 2.4 kernel.

# What? Why? How?

> What happens if I have a very old PC with MS DOS 6.0 and I want to migrate it to VirtualBox?

It's awfully simple: Use `dd` and a USB to IDE adapter...

> Unfortunately, I have a very old IDE disk that is not supported by the adapter and it donesn't works.

Another awfully simple solution: Burn `dsl-n-01RC4.iso` on a CD and boot from that ancient computer. Then run:

    dd if=/dev/hda of=/my/USB/disk/mounted/on/mnt

> Oh, my! My disk has some important info and bad blocks, but that ISO doesn't have `ddrescue`. Now what?

Not so simple. Download `ddrescue` source code and compile it on a DSL virtual machine. Then boot the live CD and...

> What? I don't want to get my hands dirty using `gcc`!

Then download the precompiled binary from this repository and run it!
