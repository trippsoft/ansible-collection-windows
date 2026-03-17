<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.windows.testing_chocolatey
Version: 1.2.0

This role configures the Testing Chocolatey Repository on Windows hosts.
It ensures that the repository is added and properly configured for use with Chocolatey package manager.


## Requirements

| Platform | Versions |
| -------- | -------- |
| Windows | <ul><li>all</li></ul> |

## Dependencies

| Collection |
| ---------- |
| chocolatey.chocolatey |

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| choco_configure_testing_repo | <p>Whether to configure the Testing Chocolatey Repository.</p> | bool | no |  | False |
| choco_testing_repo_name | <p>The name of the Testing Chocolatey Repository to be configured.</p><p>This option is required if C(choco_configure_testing_repo) is set to C(true).</p> | str | no |  |  |
| choco_testing_repo_url | <p>The URL of the Testing Chocolatey Repository to be configured.</p><p>This option is required if C(choco_configure_testing_repo) is set to C(true).</p> | str | no |  |  |


## License
MIT

## Author and Project Information
Jim Tarpley (@trippsc2)
<!-- END_ANSIBLE_DOCS -->
