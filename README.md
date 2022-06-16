OpenVPN
=========

Simple role to install OpenVPN

Requirements
------------

- Ubuntu 18+

Role Variables
--------------

first_install: false | First install flag. If 'true' - update server and install OpenVPN<br>
flush_all: false | Delete all entries<br>
update_config: false | Update server\user conf files<br>
create_user: true | Create user for OpenVPN (user.ovpn)<br>
ovpn_port: '1194'<br>
ovpn_proto: 'udp'<br>
ovpn_user: 'client'<br>
ovpn_user_file_local: '/Users/apple/Desktop'<br>

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
