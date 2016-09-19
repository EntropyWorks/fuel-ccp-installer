===========================
Vagrant for a quick dev env
===========================

Requirements:

* Vagrant >= 1.8.5
* Plugin vagrant-libvirt >= 0.0.35
* Plugin vagrant-vbguest >= 0.13.0

To start with defaults, just run ``vagrant up``. To tweak defaults, see the
`vagrant-settings.yaml_defaults` file. You can rename the file as
`vagrant-settings.yaml` end edit it to override defaults as well.

.. note:: Make sure the default network choice doesn't conflict with existing
     host networks!
.. note:: If you are running on Ubuntu Xenial, you may need to run the
   following command: ``sudo sh -c 'echo 0 > /proc/sys/net/bridge/bridge-nf-call-iptables'``
   or else container networking will be broken.
