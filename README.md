# my-raspberry-provision

An ansible role to service provision my raspberry

## System Requirements

- Raspberry Pi Model 3
- SD Card with Raspbian Stretch image, kernel version 4.9

## Usage

Specify your own variables in `inventories/hosts`:
```
[raspberry]
YOUR_STATIC_IP

[raspberry:vars]
router=YOUR_ROUTER_IP
ansible_ssh_user=YOUR_RASPBERRY_USER
```

This role will set the raspberry given ip as static.

```
ansible-playbook -i inventories/hosts provision.yml --ask-pass
```
