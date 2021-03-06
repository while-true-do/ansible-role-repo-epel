[![Build Status](https://travis-ci.org/while-true-do/ansible-role-repo-epel.svg?branch=master)](https://travis-ci.org/while-true-do/ansible-role-repo-epel)

# Ansible Role: Repo-EPEL
| A role that installs yum repository for Extra Packages for Enterprise Linux (EPEL).

## Motivation

This role is needed to get access for Extra Packages for Enterprise Linux (EPEL).

## Installation

**NOTE**: The armhfp repository is automatically rebuilt without any quality assurance or tests. Please set variable `wtd_repo_epel_armhfp_confirm` to `true` if you want to use this repository.

Install from [Ansible Galaxy](https://galaxy.ansible.com/while_true_do.repo_epel)

```
ansible-galaxy install while_true_do.repo_epel
```

Install from [Github](https://github.com/while-true-do/ansible-role-repo-epel)

```
git clone https://github.com/while-true-do/ansible-role-repo-epel.git while_true_do.repo_epel
```

## Requirements

**Used Modules**

-   [package_module](https://docs.ansible.com/ansible/latest/modules/package_module.html)
-   [yum_repository](https://docs.ansible.com/ansible/latest/modules/yum_repository_module.html)

## Role Variables
```yaml
# You can change the state (present|absent)
wtd_repo_epel_state: present
wtd_repo_epel_packages: ["epel-release"]
wtd_repo_epel_armhfp_baseurl: "https://armv7.dev.centos.org/repodir/epel-pass-1/"
wtd_repo_epel_armhfp_confirm: false

```

## Dependencies

None.

## Example Playbook

Simple Example:

```yaml
- hosts: servers
  roles:
    - { role: while_true_do.repo_epel }
```

## Testing

All tests should be put in [test directory](./tests/).

## Contribute / Bugs

Thank you so much for considering to contribute. Every contribution helps us.
We are really happy, when somebody is joining the hard work. Please have a look
at the links first.

-   [Contribution Guidelines](./docs/CONTRIBUTING.md)
-   [Create an issue or Request](https://github.com/while-true-do/ansible-role-repo-epel/issues)
-   [See who was contributing already](https://github.com/while-true-do/ansible-role-repo-epel/graphs/contributors)

## License
This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Author Information

Blog: [blog.while-true-do.org](https://blog.while-true-do.org)

Mail: [hello@while-true-do.org](mailto:hello@while-true-do.org)
