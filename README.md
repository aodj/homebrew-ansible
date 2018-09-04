Ansible 2.5.4 tap
-----------------
To install this tap, simply run `brew install aodj/ansible/ansible`

Issues
======
When installing this tap, problems may arise as time passes, wherein the Homebrew bottle that the installation process relies upon is removed from the https://homebrew.bintray.com repository (this is the case as of Sept 2018).

In this event, the installation process will attempt to install the dependencies listed in `ansible.rb` which may present issues when running against macOS; as an example, `lxml` is notoriously painful to install. If this happens, simply install `lxml` manually (ie: `pip install lxml`) and then after tapping this formula (`brew tap aodj/ansible`) comment out the `lxml` resource in the formula.