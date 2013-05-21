Start up an EC2 instance
========================

If you have an amazon code, you may want to redeem it here:

      http://aws.amazon.com/awscredits/

Go to aws.amazon.com

Go to console

Select EC2

Select "Launch Instance", and keep "Quick Launch Wizard" filled in.

Enter a name for a key pair (something simple -- lower case, no spaces)
and select "Download".  Then select "More Amazon machine images" and
"Continue."

.. image:: images/ec2-1.png
   :width: 90%

Next, enter **ami-00ca6a69** in the search box. (you might want to
copy/paste!) Continue.

.. image:: images/ec2-2.png
   :width: 90%

Make sure to select "m1.large" as the type.

.. image:: images/ec2-3.png
   :width: 90%

Select "launch."

.. image:: images/ec2-4.png
   :width: 90%

While it's launching, go to "Security groups" and modify the quicklaunch-1
group to allow HTTPS. 

.. image:: images/ec2-5.png
   :width: 90%

Briefly, select the group, then select "Inbound", then choose HTTPS
from the pull-down menu, select "Add Rule", and select "Apply rule changes".
The final list should look like the list on the right -- containing 'ssh'
and 'https'.

.. image:: images/ec2-6.png
   :width: 90%

Last, but not least: you'll want to make sure the instance is running
(green state, upper right) and you'll need the hostname of the instance
(ec2-???-???-???-???.compute-1.amazonaws.com) for the next steps.

.. image:: images/ec2-7.png
   :width: 90%

