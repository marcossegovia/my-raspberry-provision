# my-raspberry-provision

An ansible role to service provision my raspberry

## System Requirements

- Raspberry Pi Model 3
- SD Card with Raspbian Stretch image, kernel version 4.9

## Usage

```
ansible-playbook -i inventories/hosts provision.yml --ask-pass
```
