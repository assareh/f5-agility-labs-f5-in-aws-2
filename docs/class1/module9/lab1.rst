Big-IP Cloud Edition for AWS
----------------------------

From your Super-NetOps terminal run "terraform output" and note the asg-lb and web-server-x values. The asg-lb is the classic AWS load-balancer that was deployed via terraform at the beginning of the lab. You will need these values to create a service scaling group in Big-IQ.

.. code-block:: bash

   terraform output asg-lb
   terraform output web-server-1
   terraform output web-server-2

.. image:: ./images/1_elb_for_ssg_app.png
  :scale: 50%

.. image:: ./images/1a_web_servers_for_ssg_app.png
  :scale: 50%

Login to Big-IQ. Applications => APPLICATIONS => Create Application.

