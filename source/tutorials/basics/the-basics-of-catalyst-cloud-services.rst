.. _services_on_the_catalyst_cloud:

##############################
Services on the Catalyst Cloud
##############################

In the previous section, we learned that services on the Catalyst Cloud are
pieces of hardware and software that we make easy and convinent to use by
controling them with OpenStack. Now we'll learn about the various services
offered by Catalyst Cloud so that we know *what* we can do on the Catalyst Cloud,
even if right now we don't know *how* we can do it yet.

.. _compute_basics:

Compute service
===============

The compute service provides compute power on demand, in the form of "instances".
If you like to think about physical computers, you can imagine an instance as
one or more CPUs and GB of RAM that you have rented the right to use. Instances
come in many sizes, as you can see on the Catalyst Cloud's `compute page`_.

.. _`compute page`: https://catalystcloud.nz/services/iaas/compute/#prices

While you are provisioning an instance, you will pay for that instance on a per hour
basis. When you don't want the instance anymore, you can delete it, and you'll
stop paying for it. There is no minimum or maximum time you can provision an instance.
Very simple.

Keep in mind that just like a CPU is useless on it's own without an operating
system to control it, an instance needs to be attached to an operating system
to do anything useful. Don't worry, we'll talk about that later in the block
storage and image service sections.

Block storage service
=====================

The block storage service provides volumes of data storage that you can attach
to instances. You could imagine block storage volumes as hard disk drives and
solid state drives on a physical computer. Block storage volumes can be as large
or as small as you want them to be.

By attaching a volume to an instance, you mount it, making the file system
available to the CPU and memory. This could be to provide the instance
with additional storage space. Additionally, by installing operating systems
onto volumes, you can boot the attached instance into the operating system. This
is how you turn an instance from a mostly useless collection of CPU and memory
to a useful, working computer. The process of installing operating systems onto
volumes is made easier with the image service, which we'll talk about later.

You provision block storage volumes in increments of 1 GB. You pay for block storage
by the quantity of GB, multiplied by the number of hours you have provisioned them.
When you don't want the block storage volume anymore, you can delete it, and you'll
stop paying for it. You can provision a few large volumes, or provision many smaller
volumes, it's entirely up to you. There is no minimum or maximum time you can
provision a volume. Very simple.

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

An image is a "pre-made" operating system installation that can be used immediately
by an instance, rather than spending time installing the operating system, the
drivers, miscellaneous files, and configurations that help the instance integrate
better with the Catalyst Cloud. Images allow you to know that your preferred
operating system will work on the Catalyst Cloud the first time you try.

Among the operating systems provided out of the box on the Catalyst Cloud image
service are Ubuntu, Microsoft Windows 2012-2016, Debian, and CentOS. You can also
 create your own custom images to account for your own specific needs.

Linux images are free, but Windows images are priced per hour, and are priced
based on the size of the instance they are attached to.
