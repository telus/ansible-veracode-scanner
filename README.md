# ansible-veracode-scanner

[![Build Status](https://travis-ci.org/telusdigital/ansible-veracode-scanner.svg?branch=master)](https://travis-ci.org/telusdigital/ansible-veracode-scanner)
[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)

Tunables
--------
* `veracode_scanner_api_username` (string) - The API user for veracode.
* `veracode_scanner_api_password` (string) - The API password for veracode.
* `veracode_scanner_team` (string) - The name of the veracode team.
* `veracode_scanner_business_unit` (string) - The business unit for veracode.
* `veracode_scanner_business_criticality` (string) - The intensity of the veracode scan to be completed.
* `veracode_scanner_repo` (string) - The repo URL of the app to be scanned.
* `veracode_scanner_app_name` (string) - The name of the app. Usually the repo slug is sensible.
* `veracode_slack_upload` (boolean) - Upload the scan results to slack?
* `veracode_scanner_slack_token` (string) - The slack token. 
* `veracode_scanner_slack_channel` (string) - The slack channel to upload to.
* `veracode_scanner_cron_shedule` (string) - The cron shedule to run scans and slack uploads.
* `veracode_scanner_cron_user` (string) - The user to run cron as.

Dependencies
------------
[telusdigital.ruby](https://github.com/telusdigital/ansible-ruby/)

Example Playbook
----------------
    - hosts: servers
      roles:
         - role: telusdigital.veracode-scanner


License
-------
[MIT](https://tldrlegal.com/license/mit-license)

Contributors
------------
* Ben Visser
* Isaiah Thiessen
