#######################
Renaming Cloud projects
#######################

Currently the only option to rename your project in the Catalyst Cloud is by creating a
support ticket via our `Support Ticket <https://dashboard.cloud.catalyst.net.nz/management/tickets/>`_
page.

*****************
Renaming projects
*****************

Before creating a support ticket to rename a cloud project, there are some implications
you should take into consideration:

1. If you aren't interacting with the APIs directly and only using the dashboard,
   then the OpenStack project rename shouldn't affect you at all.
2. If you are using the APIs directly, then the project rename will require
   changes to configuration files for any services or tools you have talking to
   the APIs.

.. note::

  The Catalyst Cloud suggest all customers to use their project ID rather than
  the name to authenticate, otherwise after renaming their projects it will break
  their ability to authenticate until you update them to the new name.

3. You can see your project id on the API access panel by pressing the `credential
   button <https://dashboard.cloud.catalyst.net.nz/project/api_access/>`_.

If you are comfortable with the changes that may happen upon renaming your project,
send us a request via our `Support Ticket <https://dashboard.cloud.catalyst.net.nz/management/tickets/>`_.


**************
Renaming users
**************

In the Catalyst Cloud, renaming a user is the same as changing their email address.
The only way to change their user name is the user themselves change their email address by:

1. Logging into the `cloud dashboard <https://dashboard.cloud.catalyst.net.nz/settings/email/>`_
2. After logging in, click on your user name at the right top corner of the screen
3. Select "Settings"
4. Selecting "Update Email Address"
5. Following the instructions on the screen
