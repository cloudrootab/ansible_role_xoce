# ansible_role_xoce
An Ansible role to handle the download and compilation of Xen Orchestra - Community Edition from source

> [!CAUTION]  
> DISCLAIMER!
> This is produced and offered _as is_ without **any** warranty. Made to run on Debian/Ubuntu. Do your own due diligence and verify the code/functions.
> No guarantees are given nor are any responsibilities taken. NONE!
> No support is offered!
> **Use at your own risk!**

### Standing on the shoulders of giants
This wouldn't be possible without the awesome work done by Vates and the open source community in large. Please help out by contributing in some way to this great project.
If you have any questions. Please refer to the official docs: [https://docs.xen-orchestra.com/](https://docs.xen-orchestra.com/). Or consider purchasing their paid support through their [XOA](https://xen-orchestra.com/) support packages. 

#### Background
This is something I've thrown together and been using for the better part of a year. 

#### Benefits _vs_ the many scripts available
Those scripts are often quite involved and have grown quite big. Making them hard to scrutinize and validate so that they _acctually_ do what they claim to do. More importantly so that they don't do something they _shouldn't_. For this I preffer to use Ansible. As this in my oppinion makes everything more standardized and easier to read.

#### Requirements
* Debian based system. Tested and used on Ubunutu.
* Installs node.js from nodesource.com's repo, using apt. (Currently LTS-24)

> [!NOTE]  
> This sets up the `xo-server` to run as non-root, using sudo. This _should_ improve security further.
> But this means that the webserver port defaults to `8443`

##### Known-Issues:
* There could be a permission problem when mounting SRs on new installs.
* Probably several others. But I don't remember.
