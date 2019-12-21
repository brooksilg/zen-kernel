# Zen Kernel with Nitrocaster FHD mod patches

This is a fork of the [`zen-kernel`](https://github.com/zen-kernel/zen-kernel) with [this kernel patch](https://pastebin.com/WF6wdfpb) applied.

More information about the Nitrocaster FHD mod can be found on [this thinkpads.com forum topic](https://thinkpads.com/forum/viewtopic.php?f=43&t=122640).

**Note:** Before compiling this kernel for your x230, make sure the `DMI_PRODUCT_NAME` matches your personal machine:
1. Run `dmesg | grep DMI` and copy your specific DMI string
1. Update `DMI_PRODUCT_NAME` for the "Thinkpad X230 Nitrocaster Mod" entry found in [`/drivers/gpu/drm/i915/display/intel_lvds.c` (view)](https://github.com/brooksilg/zen-kernel/blob/HEAD/drivers/gpu/drm/i915/display/intel_lvds.c#L719)


Linux kernel
============

There are several guides for kernel developers and users. These guides can
be rendered in a number of formats, like HTML and PDF. Please read
Documentation/admin-guide/README.rst first.

In order to build the documentation, use ``make htmldocs`` or
``make pdfdocs``.  The formatted documentation can also be read online at:

    https://www.kernel.org/doc/html/latest/

There are various text files in the Documentation/ subdirectory,
several of them using the Restructured Text markup notation.

Please read the Documentation/process/changes.rst file, as it contains the
requirements for building and running the kernel, and information about
the problems which may result by upgrading your kernel.
