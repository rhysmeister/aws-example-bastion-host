# aws-example-bastion-host
An example AWS project creating a Bastion host

* 1 Region, 3 AZs.
* ASG used to ensure there is always one Bastion host running.
* Clout Init yaml file used to bootrap the Bastion host.

# AWS Setup Prerequisites

* https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-prereqs.html
* https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-prereqs-self-managed.html#stacksets-prereqs-accountsetup

# Possible enhacements

The following improvements are suggested for production usage...

* Create an EIP for the Bastion host, or do something in Route 53, to allow for easier connectivity.
* Mount an EFS volume to provide a space to save files on the Bastion host that is not destroyed between Bastion host instance.
* Additional Parameter Inputs.