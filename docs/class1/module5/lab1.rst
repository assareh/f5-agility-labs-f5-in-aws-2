Create an IPSec VPN between an F5 Big-IP appliance and AWS
----------------------------------------------------------

From the Linux terminal app, open a new tab. Invoke the "bigip" shell alias command to ssh to your on-premises bigip1.

.. code-block:: bash

   bigip
   default

From bigip1, use dig to discover the public IP address assigned to your bigip1.

.. code-block:: bash

   dig -b 10.1.20.11 TXT +short o-o.myaddr.l.google.com @ns1.google.com

.. image:: ./images/1_bigip1_publicip.png
  :scale: 50%
