# How to deploy a Gluster cluster end-to-end?

The cluster-vars.yml file contains variables for setting the backend disks using
LVM thinpool and creating a Gluster volume. The example playbook creates a
replica 2 volume with 4 bricks (2x2), but any volume type can be created.
Please refer: https://github.com/gluster/gluster-ansible-cluster

## Usage:
To run the playbook create an inventory file containing the hosts in question.
Edit the inventory file to suit your needs. And run the playbook:

```
$ ansible-playbook -i path-to-inventory gluster_volume.yml

```
