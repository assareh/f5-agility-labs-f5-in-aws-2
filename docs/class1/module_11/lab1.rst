Clean up the lab environment
----------------------------

.. attention::
   
   Lab testers: this is the most important step. Please clean-up.
   

.. image:: ./images/1_delete_apps.png
  :scale: 50%

.. image:: ./images/2_delete_ssg.png
  :scale: 50%

.. image:: ./images/3_ssg_cfg_gone.png
  :scale: 50%

.. image:: ./images/4_delete_vpn.png
  :scale: 50%

.. image:: ./images/5_delete_customer_gw.png
  :scale: 50%

.. code-block:: bash

   terraform destroy --force

.. image:: ./images/6_terraform_destroy.png
  :scale: 50%

.. image:: ./images/7_terraform_destroy_done.png
  :scale: 50%

.. image:: ./images/8_aws_terminated.png
  :scale: 50%