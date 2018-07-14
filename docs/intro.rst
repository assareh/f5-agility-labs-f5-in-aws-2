Getting Started
---------------

Your instructor will provide URL where you can access your lab environment.

.. NOTE::
	 All work for this lab will be performed exclusively from the Linux jumphost. No installation or interaction with your local system is required.

Lab Topology
~~~~~~~~~~~~

Before you start the lab you will have an empty environment.  You will be building out the following topology.

Network Topology
^^^^^^^^^^^^^^^^^

.. image:: /_static/f5-public-cloud-network-toplogy.png
  :scale: 50%

The following components will be built in your lab environment:

- 1 x F5-BIG VE WAF (v13.1)
- 2 x Linux Webserver (Amazon Linux AMI)

Automation Tools
~~~~~~~~~~~~~~~~

During the lab you will be using multiple automation tools.

Without these automation tools you would be required to perform many tasks in precise sequence.

.. image:: /_static/no-automation.png
  :scale: 25%

Using Automation we can simplify this proces to create a faster, safer, and more secure solution.

.. image:: /_static/automation-pipeline.png
  :scale: 25%

By chaining together multiple declarative interfaces and tools.

.. image:: /_static/declarative-interfaces.png
  :scale: 25%


HashiCorp Terraform
^^^^^^^^^^^^^^^^^^^

HashiCorp Terraform is used to create the underlying Network environment, deploy the Linux Webservers, and deploy F5 BIG-IP via AWS Cloud Formation Templates.

Amazon Cloud Formation Templates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Amazon Cloud Formation Templates (CFT) are used to deploy F5 BIG-IP resources.  In addition to deploying the F5 BIG-IP VE, the CFT template also manages Elastic Network Interfaces (ENI), Security Groups, EC2 Instance Roles, and other cloud native services.

F5 Provides Supported Cloud Formation Templates that customers can leverage in their AWS environments.  The lab will deploy:

An F5 Virtual Edition WAF behind an AWS Application Load Balancer. The F5 Virtual Edition WAF will be protecting our pool of 2 x example applications.

F5 Super NetOps Container
^^^^^^^^^^^^^^^^^^^^^^^^^^

To simplify the installation of these Automation Tools (Terraform/CFT) we will use the F5 Super NetOps Container to provide a consistent environment for running the lab.

Connecting to the Lab Environment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Your instructor will provide directions on how to connect to the Ravello Portal.
