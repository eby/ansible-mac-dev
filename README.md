## My Setup for personal Macs

This uses ansible to install apps and settings for my personal setup in case a reinstall is needed. 

### To Run
    $ xcode-select --install
    $ sudo easy_install pip
    $ sudo pip install ansible
    $ mkdir projects && cd projects
    $ git clone git@github.com:eby/ansible-mac-dev.git
    $ cd ansible-mac-dev
    $ ansible-galaxy install -r requirements.yml
    $ ansible-playbook -i inventory --ask-become-pass main.yml 
