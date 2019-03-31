Experitest - File Storage ansible role
=========

This role will install \ uninstall file storage for mac os hosts

Requirements
------------

This role assumes that you have java 8 installed on the instance
Supports mac os hosts only.

Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| state | should the application be present or absent | present, absent | present | no |
| app_version | application version to install | string | 12.4.5403 | no |
| server_port | port number for the server | number | 8082 | no |
| extra_app_props | additional props to be override in application.properties file | dict | {} | no |
| installation_folder | the folder in which the applction will be installed | string | for mac: ~/experitest/file-storage-version <br> for windows: C:\\Experitest\\file-storage-version  | no |
| jmx_port | port number for jmx inspection | number | 51236 | no |
| custom_download_url | custom url to download the installation from (zip format) | string |  | no |
| start_after_install | should application start after installation is completed | boolean | True | no |
| clear_temp_folder | remove temp folder after installation | boolean | False | no |
| file_storage_folder | folder that will contain the data | string | for mac: ~/experitest/file-storage-content <br> for windows: C:\\ProgramData\\file-storage-content  | no |
| clear_before_install | removing old installation before installing new version | boolean | False | no |

Example Playbook
----------------

#### [see working example](/example)
