# vagrant-bazel

This repository is for quickly spinning up an Ubuntu trusty-tar 64bit box
with [Bazel](https://bazel.build/), Google's new build tool.

### Prerequisities

The following software stack will need to be installed in order to setup the
environment.

* [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Ansible](https://docs.ansible.com/ansible/intro_installation.html#getting-ansible)

### Standing up the environment

Once everything all the pre-reqs are installed, you simply need to run the
following command:

> This is assuming a \*nix environment

```bash
vagrant up
```

This should download Ubuntu14.04, and execute ansible in order to install
all of the necessary dependencies to run Bazel.

##### Selecting a Bazel version

The Bazel version that is installed can be modified by changing the
`bazel_version` variable in [playbook.yml](https://github.com/skippyPeanutButter/vagrant-bazel/blob/master/playbook.yml#L4).

See the list of Bazel releases [here](https://github.com/bazelbuild/bazel/releases)
