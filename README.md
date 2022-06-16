OpenVPN
=========

Simple role to install OpenVPN

Requirements
------------

- Ubuntu 18+

Role Variables
--------------

first_install: false | First install flag. If 'true' - update server and install OpenVPN
flush_all: false | Delete all entries
update_config: false | Update server\user conf files
create_user: true | Create user for OpenVPN (user.ovpn)

ovpn_port: '1194'
ovpn_proto: 'udp'
ovpn_user: 'client'
ovpn_user_file_local: '/Users/apple/Desktop'

Dependencies
------------

Role no requier any dependencies

Example Playbook
----------------

- name: Openvpn
  hosts: openvpn
  roles:
    - role: '{{playbook_dir}}'

License
-------

BSD

Author Information
------------------

Sobolev Maxim
