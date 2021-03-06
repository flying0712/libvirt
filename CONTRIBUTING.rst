=======================
Contributing to libvirt
=======================

Full, up to date information on how to contribute to libvirt can be
found on the libvirt website:

https://libvirt.org/contribute.html

To build the same document locally, from the top level directory of
your git clone run:

::

  $ mkdir build && cd build
  $ ../autogen.sh
  $ make

You'll find the freshly-built document in ``docs/contribute.html``.

If ``configure`` fails because of missing dependencies, you can set
up your system by calling

::

  $ sudo dnf builddep libvirt

if you're on a RHEL-based distribution or

::

  $ sudo apt-get build-dep libvirt

if you're on a Debian-based one.

You might still be missing some dependencies if your distribution is
shipping an old libvirt version, but that will get you much closer to
where you need to be to build successfully from source.
