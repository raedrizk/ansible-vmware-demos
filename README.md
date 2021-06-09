# ansible-vmware-demos

Ansible collection (`rsoliman.vmware_demos`) containing some roles to demonstrate using ansible to automate common vmware tasks, as well as sample playbooks that call on those roles.

Playbooks included in this repo:

- vmware_create_ESXI_inventory.yml
- vmware_create_snapshot.yml
- vmware_delete_snapshot.yml
- vmware_restore_snapshot.yml
- vmware_create_vm_from_template.yml
- vmware_delete_vm.yml
- vmware_find_default_vm_folder.yml


The `rsoliman.vmware_demos` collection has a dependancy on the modules from the following collections:
- `community.vmware`
- `vmware.vmware_rest`
- `awx.awx`
- `ansible.builtin`

To use the playbooks in Ansible tower:

1. create a new project pointing to this repo
2. define credentials for vcenter and Tower
3. create job templates to use the playbooks you need