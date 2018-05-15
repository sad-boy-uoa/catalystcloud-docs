.. _services_on_the_catalyst_cloud:

##############################
Services on the Catalyst Cloud
##############################

In the previous section, we learned that services on the Catalyst Cloud are
pieces of hardware that we make easy and convinent to use by controling them
with OpenStack. Now we'll learn about the various services offered by Catalyst
Cloud so that we know *what* we can do on the Catalyst Cloud, even if right now
we don't know *how* we can do it.

.. _compute_basics:

Compute service
===============

The compute service provides compute power on demand, in the form of "instances".
If you like to think about physical computers, you can imagine an instance as
one or more CPUs and GB of RAM that you have rented the right to use. Instances
come in many sizes, as you can see on the Catalyst Cloud's `compute page`_.

.. _`compute page`: https://catalystcloud.nz/services/iaas/compute/#prices

While you are renting an instance, you will pay for that instance on a per hour
basis. When you don't want the instance anymore, you can delete it, and you'll
stop paying for it. There is no minimum or maximum time you can rent an instance.
Very simple.

Keep in mind that just like a CPU is useless on it's own without an operating
system to control it, an instance needs to be attached to an operating system
to do anything useful. Don't worry, we'll talk about that later in the block
storage and image service sections.

Block storage service
=====================

The block storage service provides volumes of data storage that you can attach
to instances. On a physical computer, you can imagine block storage volumes as
hard disk drives and solid state drives. Block storage volumes can be as large
or as small as you want them to be. 
