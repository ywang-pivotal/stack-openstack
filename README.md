# OpenStack High-Availability Cookbook

This cookbook is an automation framework that can be used to setup enterprise grade highly available OpenStack
environments. The goal of this framework is to be able to describe a distributed OpenStack deployment in a template
which can be shared with the community. It captures these various OpenStack topologies in templates, which can be
executed in a repeatable manner.

## Supported Platforms

TODO: ...

## Installation

You can run this framework by installing the required Chef configuration tools within your rvm/rubyenv environments
or within a ChefDK environments. The recommended approach described below sets up the required additional tools
within a ChefDK environment.

1. First download and install the latest [ChefDK](https://downloads.getchef.com/chef-dk/). This will give you a self
contained ruby environment. If you have other ruby environments managed by rvm/rubyenv, you can manage which one to
use based on your current directory using [direnv](http://direnv.net/).

2. Install the knife-stackbuilder gem.

	```
	$ gem install -​-no-document knife-stackbuilder
	```
3. Clone this repository

	```
	$ git clone https://github.com/mevansam/openstack-ha-cookbook.git
	$ cd openstack-ha-cookbook
	```
4. If you plan to execute the vagrant templates then you need to get the updated
[knife-vagrant2](https://github.com/makern/knife-vagrant2) plugin for knife and the
[vagrant-ohai](https://github.com/avishai-ish-shalom/vagrant-ohai) plugin for vagrant.

	```
	$ gem install --no-document vagrant-plugins/knife-vagrant2-0.0.5.gem
	$ vagrant plugin install vagrant-plugins/vagrant-ohai-0.1.8.gem
	```
    > These patches and updates are in the process being pushed to their respective upstream repositories. The patched gems are available at:
    > * [knife-vagrant2](https://github.com/mevansam/chef-knife-vagrant2.git)
    > * [vagrant-ohai](https://github.com/mevansam/vagrant-ohai.git)



### OpenStack KVM on Vagrant Template

![Image of OpenStack KVM setup on Vagrant]
(docs/images/vagrant_kvm.png)

### OpenStack KVM on VMWare Template

TODO: ...

### OpenStack HA KVM Template

TODO: ...

### OpenStack HA VMWare ESX Template

TODO: ...

### OpenStack HA XenServer Template

TODO: ...

### OpenStack HA HyperV Template

TODO: ...

### OpenStack HA Multi-Hypervisor Template

## Design

TODO: ...

## Extending

TODO: ...

## Contributing

1. Fork the repository on Github
2. Create the
5. Submit a Pull Request

## License and Authors

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Author | Email | Company
-------|-------|--------
Mevan Samaratunga | msamaratunga@pivotal.io | [Pivotal](http://www.pivotal.io)
