# lib_openshift

OpenShift Ansible has a number of ansbile roles that are quite useful and not yet in Ansible Galaxy

https://github.com/openshift/openshift-ansible/tree/master/roles/lib_openshift

```
git clone https://github.com/openshift/openshift-ansible
cp -R ~/git/openshift-ansible/roles/lib_openshift roles/ # not in galaxy yet
```

Example usage: Creating a namespace

```
ansible-playbook -vv main.yaml
```