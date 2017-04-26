# Ansible Role: malesgan

Install various package on centos 7, because I'm too lazy to do it manually

## Repo
    - ius repo
    - epel-release
    - mongodb-org-3.4

## Package
    - autoconf
    - automake
    - bison
    - byacc
    - cscope
    - ctags
    - elfutils
    - flex
    - gcc-c++
    - gcc
    - gettext
    - git
    - intltool
    - kernel-devel
    - libtool
    - make
    - mariadb
    - nano
    - nginx
    - openssl-devel
    - patch
    - patchutils
    - pkgconfig
    - systemtap
    - tree
    - vim
    - wget
    - mongodb-3.4
    - php56u
    - php56u-cli
    - php56u-common
    - php56u-fpm
    - php56u-fpm-nginx
    - php56u-imap
    - php56u-mbstring
    - php56u-mcrypt
    - php56u-mysqlnd
    - php56u-gd

## Shell toolkit
  - gvm (golang version manager)

## Programming Language
  - golang 1.7.3

# Requirements

This role only is needed/runs on RHEL and its derivatives.

# Role Variables

Available variables are listed on `defaults/main.yml`

# Dependencies
  - geerlingguy.repo-epel
  - geerlingguy.redis

# Example Playbook

```
---
- hosts: all
  pre_tasks:
    - set_fact:
        ansible_distribution_major_version: "7"

  gather_facts: true
  roles:
    - { role: widnyana.malesgan, become: yes }
```

# License

MIT / BSD

# Author Information
This role was created in 2017 by [Widnyana](https://github.com/widnyana)