# ansible-role-rally

An Ansible role to install, configure and run Rally OpenStack test suite

## Role Variables

This is the list of role variables:

  * `rally_result_filename`: Name of the generated file. Default to `rally.xml`.
  * `rally_scenario_filepath`: The path to the rally scenario file. Default to `/home/stack/rally-tasks.yml`
  * `rally_file_location`: (optional) URL of the rally scenario file.


## Dependencies

None.


## Example Playbook

The simplest way to use this module:

```
- name: Run the OpenStack Rally test suite
  hosts: undercloud
  vars:
    rally_file_location: https://example.com/path/to/rally-scenarios.yml
  roles:
    - rally
```

## License

Apache 2.0


## Author Information

Distributed-CI  <distributed-ci@redhat.com>
