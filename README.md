# centos 8 to centos 8 stream playbook

## Scope

This is a automated way to update a centos 8 to centos 8 stream (one way).

## Usage

```bash
ansible-playbook -i hosts -u root -k playbook/main.yaml
```

The best way to verify is to check that the `Stream` repositories are in your 
`/etc/yum.repos.d/` directory. For instance:
```bash
$ ls /etc/yum.repos.d/
CentOS-AppStream.repo   CentOS-fasttrack.repo         CentOS-Stream-centosplus.repo  CentOS-Stream-RT.repo
CentOS-Base.repo        CentOS-HA.repo                CentOS-Stream-Debuginfo.repo   CentOS-Stream-Sources.repo
CentOS-centosplus.repo  CentOS-Media.repo             CentOS-Stream-Devel.repo       CentOS-Stream-Vault.repo
CentOS-CR.repo          CentOS-PowerTools.repo        CentOS-Stream-Extras.repo      CentOS-Vault.repo
CentOS-Debuginfo.repo   CentOS-Sources.repo           CentOS-Stream-HA.repo
CentOS-Devel.repo       CentOS-Stream-AppStream.repo  CentOS-Stream-Media.repo
CentOS-Extras.repo      CentOS-Stream-Base.repo       CentOS-Stream-PowerTools.repo
```

## Tested on

This has been tested and works on:
- CentOS 8

## Author and Licence

Author: JJ Asghar <awesome@ibm.com>

```text
Copyright:: 2020- IBM, Inc

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
