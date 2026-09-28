# incus

## Description

This repository contains spec files for building `incus` RPM packages and its dependencies.

Packages are built and published by [spec-package-builder](https://github.com/damex-el-packages/spec-package-builder) pipeline.

Currently, packages and their corresponding spec files are built and tested only for `Red Hat Enterprise Linux 9`, `Red Hat Enterprise Linux 10` and its derivatives like `Alma Linux 9`, `Alma Linux 10`, `Rocky Linux 9` and `Rocky Linux 10`.

[Follow here if you want to use prebuilt packages](#Using-prebuilt-packages).

## Using prebuilt packages

### Add damex-incus repository with prebuilt packages

To add `damex-incus` repository to `Red Hat Enterprise Linux 9` install the following package:

```sh
# x86_64
https://yum-repositories.damex.org/incus/el/9/x86_64/damex-incus-release-0.2.0-1.el9.x86_64.rpm
# aarch64
https://yum-repositories.damex.org/incus/el/9/aarch64/damex-incus-release-0.2.0-1.el9.aarch64.rpm
```

To add `damex-incus` repository to `Red Hat Enterprise Linux 10` install the following package:

```sh
# x86_64
https://yum-repositories.damex.org/incus/el/10/x86_64/damex-incus-release-0.2.0-1.el10.x86_64.rpm
# aarch64
https://yum-repositories.damex.org/incus/el/10/aarch64/damex-incus-release-0.2.0-1.el10.aarch64.rpm
```

Alternatively, it can be done manually by adding the following configuration to `/etc/yum.repos.d/damex-incus.repo`:

```sh
[damex-incus]
name = damex-incus
baseurl = https://yum-repositories.damex.org/incus/el/$releasever/$basearch
gpgcheck = 1
repo_gpgcheck = 1
gpgkey = https://yum-repositories.damex.org/incus/incus-2036-09-25.asc
```

### List of prebuilt packages

| Package              | Repository | Architecture | Distributives              |
|----------------------|------------|--------------|----------------------------|
| cowsql               | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| cowsql-devel         | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| incus                | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| incus-agent          | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| incus-client         | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| incus-tools          | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| lxc                  | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| lxc-devel            | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| lxc-libs             | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| lxc-templates        | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| lxcfs                | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| raft                 | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
| raft-devel           | damex-incus | x86_64, aarch64 | Red Hat Enterprise Linux 9, Red Hat Enterprise Linux 10 |
