[![Build Status](https://travis-ci.org/while-true-do/ansible-role-repo-epel.svg?branch=master)](https://travis-ci.org/while-true-do/ansible-role-repo-epel)

# Ansible Role: Repo-EPEL
| A role that installes yum repository for Extra Packages for Enterprise Linux (EPEL).

- If wtd_repo_epel_enabled is set to false it will remove rpm package and its repository files.

## Motivation

This role is needed to get access for Extra Packages for Enterprise Linux (EPEL).

## Installation

Install from [Ansible Galaxy](https://galaxy.ansible.com/while-true-do.repo-epel)

```
ansible-galaxy install while-true-do.repo-epel
```

Install from [Github](https://github.com/while-true-do/ansible-role-repo-epel)

```
git clone https://github.com/while-true-do/ansible-role-repo-epel.git while-true-do.repo-epel
```

## Requirements

**Used Modules**

-   [package_module](http://docs.ansible.com/ansible/latest/package_module.html)

## Role Variables
```yaml
# You can change the state (present|absent)
wtd_repo_epel_state: present
wtd_repo_epel_packages: ["epel-release"]

```

## Dependencies

None.

## Example Playbook

Simple Example:

```yaml
- hosts: servers 
  roles:
    - { role: while-true-do.repo-epel }
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
