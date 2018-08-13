# lib_openshift

OpenShift Ansible has a number of ansbile roles that are quite useful and not yet in Ansible Galaxy

https://github.com/openshift/openshift-ansible/tree/master/roles/lib_openshift

```bash
git clone https://github.com/openshift/openshift-ansible
cp -R ~/git/openshift-ansible/roles/lib_openshift roles/ # not in galaxy yet
```

`Example`

Create a project/namespace

```bash
ansible-playbook -vv main.yaml
```

See the generated doco for usage:

```bash
roles/lib_openshift/src/doc/project

- name: create ops project
  oc_project:
    state: present
    name: openshift-ops
    display_name: operations team project
    node_selector:
    -  top=secret
    -  noncustomer=True
```