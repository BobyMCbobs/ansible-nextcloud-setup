# Setup Nextcloud via Ansible on openSUSE Leap or Ubuntu hosts
An automated approach for setting up Nextcloud on openSUSE Leap or Ubuntu  

## Requires
Ansible v2.7 or greater

## Setup
Make a hosts group in `/etc/ansible/hosts`, something like what's in `hosts`.  

Make sure you modify variables in `group_vars/all` to configure it how you like.  

## Usage
`ansible-playbook site.yml`  
or for local `hosts` use `ansible-playbook -i hosts site.yml`

## Notes
On some openSUSE systems (such as JeOS), you may have to install `kernel-default` manually in order to install the full kernel (via downgrading) with squashfs support.
