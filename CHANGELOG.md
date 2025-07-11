# Changelog

All notable changes to this project will be documented in this file.

## [1.1.3] - 2024-06-11

### Collection

- Changed repository URL to use GitHub Organization.
- Corrected missing or extra dependencies.

## [1.1.2] - 2024-02-09

### Module Plugin - wds_boot_image

- Reverted changing documentation from .py file to .yml file because ansible-lint does not parse it correctly yet.

### Module Plugin - wds_initialize

- Reverted changing documentation from .py file to .yml file because ansible-lint does not parse it correctly yet.

### Module Plugin - win_combine_certificates

- Reverted changing documentation from .py file to .yml file because ansible-lint does not parse it correctly yet.

### Module Plugin - win_package_provider

- Reverted changing documentation from .py file to .yml file because ansible-lint does not parse it correctly yet.

## [1.1.1] - 2024-02-09

### Module Plugin - wds_boot_image

- Made several code quality and style changes to the module that were recommended by the Ansible sanity tests.

### Module Plugin - wds_initialize

- Made several code quality and style changes to the module that were recommended by the Ansible sanity tests.

### Module Plugin - win_combine_certificates

- Made several code quality and style changes to the module that were recommended by the Ansible sanity tests.

### Module Plugin - win_package_provider

- Made several code quality and style changes to the module that were recommended by the Ansible sanity tests.

## [1.1.0] - 2024-01-25

### Collection

- *wds_boot_image* module plugin added.
- *wds_initialize* module plugin added.

### Role - deployment_services

- Removed boot images from the role to keep it idempotent. This functionality should be moved outside the role using the *wds_boot_image* module plugin.
- Replaced WdsDsc resource for initializing the WDS server with *wds_initialize* module plugin.

## [1.0.7] - 2024-01-08

### Collection

- Added Changelog.
- Updated collection README documentation.

## [1.0.6] - 2024-10-22

### Role - install_psgallery

- Removed `os_family` subset for fact gathering step as it is not used on Windows machines.

## [1.0.5] - 2024-09-06 

### Role - deployment_services

- Added the `no_log` option for the `wds_admin_password` variable.

## [1.0.4] - 2024-08-09

### Collection

- Minimum Ansible version changed from `2.14` to `2.15` due to EOL status.

## [1.0.3] - 2024-07-12

### Role - dhcp_server

- Updated documentation and role metadata for readability.
- Added the `dhcp_install_management_tools` variable to enable/disable installing DHCP management tools.
- Renamed the `dhcp_options` variable to `dhcp_server_options` variable.
- Added validation for variables where possible.

## [1.0.2] - 2024-06-30

### Collection

- Added dependency reference to **ansible.windows**.
- Added dependency reference to **community.windows** with a version requirement of `>=1.11.0`.

### Role - dhcp_server

- Fixed documentation to properly include role dependencies.

## [1.0.0] - 2024-06-24

### Collection

- Initial release.
- *win_combine_certificates* module plugin added.
- *win_package_provider* module plugin added.
- *deployment_services* role added.
- *dhcp_server* role added.
- *install_psgallery* role added.
