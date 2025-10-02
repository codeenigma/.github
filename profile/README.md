## Code Enigma

### 🦊 Public Service Announcement
We are starting to migrate most of our work to GitLab due to reliability issues here on GitHub. [You can follow us over there via this link.](https://gitlab.com/code-enigma)

We are [Code Enigma](https://www.codeenigma.com/), a community of creative souls and the technically brilliant, dedicated to building a better world wide web. Our GitHub is where we share things we think might be useful to everybody.
This is mostly about supporting developers to do better work. For more information visit [ce.tools](https://ce.tools).
To reach out you can toot at us 🦣 via [toots.codeenigma.com/@codeenigma](https://toots.codeenigma.com/@codeenigma).

Our main contributions are as follows:

### ⌨️ [ce-dev](https://github.com/codeenigma/ce-dev)
This is a wrapper for [Docker Compose](https://docs.docker.com/compose/) that allows you to quickly run up local development environments with [Docker](https://www.docker.com/).
It provides some template projects and layouts but also allows for total customisation and for you to create and push your own container layouts for your projects.
This is **not** a replacement for products like `ddev`, because it simply wraps Docker to make starting and deploying a set of containers much easier.
Consequently it's less opinionated and far more customisable.

### 🚚 [ce-provision](https://github.com/codeenigma/ce-provision)
This is a set of bash scripts and [Ansible](https://www.ansible.com/) roles for managing software on Linux servers, specifically [Debian Linux](https://www.debian.org/), though wider support may follow.
It aims to be platform agnostic, although as [AWS partners](https://partners.amazonaws.com/partners/0010L00001pDHc8QAG/Code%20Enigma) we ship a lot of AWS automation for orchestrating infrastructure. Again, more providers may be added.
It can work with any CI, though we typically run it from [GitLab CI](https://docs.gitlab.com/ee/ci/) using a shell runner and using the provided shell scripts to exectute Ansible and build things.

### 🚀 [ce-deploy](https://github.com/codeenigma/ce-deploy)
This is a set of bash scripts and [Ansible](https://www.ansible.com/) roles for deploying applications to servers. It works in much the same way as `ce-provision` but the roles focus on delivering software on to servers and containers.

### 🧰 Other tools
There are some other bits in here, mainly:
* [ce-contrib-tools](https://github.com/codeenigma/ce-contrib-tools) - some bash scripts to make managing our [Git](https://git-scm.com/) workflow easier
* [ce-lightsail-launcher](https://github.com/codeenigma/ce-lightsail-launcher) - a pre-prepared [cloud-init](https://cloud-init.io/) script for quickly deploying applications to [AWS Lightsail](https://aws.amazon.com/lightsail/) servers
* [ce-provision-templates](https://github.com/codeenigma/ce-provision-templates) - a growing collection of example Ansible variables for different `ce-provision` servers and infras
* [newsletters](https://github.com/codeenigma/newsletters) - our archive of newsletters!

There are also various config templates for `ce-provision` and `ce-deploy` available to browsers of our GitHub.

### 💙 Drupal
It would be remiss of us not to mention  is how we all got here. Since 2010 we have been leading UK Drupal experts and we continue to spend most of our time supporting organisations running Drupal websites.
You can read more about our Drupal lives on [our Drupal profile](https://www.drupal.org/code-enigma).

Drupal modules aside, you'll find some other PHP gems in our repos:
* [ce_ldap](https://github.com/codeenigma/ce_ldap) - a [Drupal](https://www.drupal.org/) module for syncing [LDAP](https://www.openldap.org/) users on a schedule
* [ce_localgovdrupal_config](https://github.com/codeenigma/ce_localgovdrupal_config) - a [Drupal](https://www.drupal.org/) setup config to make it quicker and easier to get [LocalGov Drupal](https://localgovdrupal.org/) up and running
* [linotp2](https://github.com/codeenigma/linotp2) - a fork of the unmaintained `linotp-auth-simplesamlphp` project providing [SimpleSAMLphp](https://simplesamlphp.org/) support for a second factor of authentication via [LinOTP](https://www.linotp.org/)
* [CE2FA](https://github.com/codeenigma/ce2fa) - another [SimpleSAMLphp](https://simplesamlphp.org/) module, allowing direct integration with the [Yubico](https://www.yubico.com/) API for Yubikeys
