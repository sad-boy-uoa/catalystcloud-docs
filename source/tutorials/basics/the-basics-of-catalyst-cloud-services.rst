.. _services_on_the_catalyst_cloud:

##############################
Services on the Catalyst Cloud
##############################

In the previous section, we learned that services on the Catalyst Cloud are
pieces of hardware and software that we make easy and convinent to use by
controling them with OpenStack. Now we'll learn about the various services
offered by Catalyst Cloud so that we know *what* we can do on the Catalyst
Cloud, even if right now we don't know *how* we can do it yet.

****************************************
What services are on the Catalyst Cloud?
****************************************

Compute service
===============

The compute service provides compute power on demand, in the form of
"instances". If you like to think about physical computers, you can imagine an
instance as one or more CPUs and GB of RAM that you have rented the right to
use. Instances come in many sizes, as you can see on the Catalyst Cloud's
`compute page`_.

.. _`compute page`: https://catalystcloud.nz/services/iaas/compute/#prices


Block storage service
=====================

The block storage service provides volumes of data storage that you can attach
to instances. You could imagine block storage volumes as hard disk drives and
solid state drives on a physical computer. Block storage volumes can be as large
or as small as you want them to be.

By attaching a volume to an instance, you mount it, making the file system
available to the CPU and memory.

Block volumes are automatically replicated multiple times across the data centre
to make your data very durable, and very available.

Network service
===============

The network service allows you to perform networking tasks easily, flexably, and
quickly. You are given the ability to create, edit, assign, and delete the basic
elements of a network, like:

* Private networks;
* Sub-networks;
* Routers;
* Firewalls (called security groups);
* IP addresses;
* Site-to-site VPNs.

Image service
=============

It is a common task to install an operating system onto a block storage volume,
so that you can boot the instance into the operating system. The image service
was created to make this as easy as possible.

An image is a "pre-made" operating system installation that can be used
immediately by an instance, rather than spending time installing the operating
system, the drivers, miscellaneous files, and configurations that help the
instance integrate better with the Catalyst Cloud. Images allow you to know that
your preferred operating system will work on the Catalyst Cloud the first time
you try.

Among the operating systems provided out of the box on the Catalyst Cloud image
service are Ubuntu, Microsoft Windows 2012-2016, Debian, and CentOS. You can
also create your own custom images to account for your own specific needs.

Object storage service
======================

Object storage is a storage system unique to cloud computing. Instead of
provisioning a volume of storage capacity, you just upload a file, and Catalyst
Cloud handles it's storage.

One of object storage's biggest advantages is it's price. As an illustration,
imagine you're provisioning a block storage volume for a database. Many of the
bits you've provisioned within that volume are unused 0s, not yet used by the
database to store any data. With object storage, you only pay for bits your
files are using, not any empty, unproductive bits. This allows you to minimise
your costs. Secondarily, data stored in object storage can be more efficently
stored than block storage, allowing Catalyst Cloud to charge less for it.

******************************
What can you do with services?
******************************

Catalyst Cloud is an entirely automated platform that adheres to the NSIT
definition of `true cloud computing <https://csrc.nist.gov/publications/d
etail/sp/800-145/final>`_. That means Catalyst Cloud
