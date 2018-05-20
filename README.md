# olddrescue

A ddrescue static binary that runs on 2.4 kernel.

# What? Why? How?

> What happens if I have a very old PC with MS DOS 6.0 and I want to migrate it to VirtualBox?

Simply use `dd` and a USB to IDE adapter...

> Unfortunately, I have a very old IDE disk that is not supported by the adapter.

Burn `dsl-n-01RC4.iso` on a CD and boot DSL-n from that ancient computer.
Then use `dd` to copy the HDD into a USB drive or a CD.

> Oh, my! My disk has some important info but has many bad blocks.
> Also I noticed that the ISO doesn't have `ddrescue`. What can I do?

Not so simple, because the DSL kernel is a ancient one and doesn't support the new `ddrescue` binaries.
You may need to run DSL-n in a virtual machine to compile a static binary for ancient kernels.

> What? I don't want to get my hands dirty using `gcc`!

Then download the precompiled binary from this repository and run it!
