Role Name
=========

Install the Lacework Datacollector Agent


Role Variables
--------------

Required

lacework_accessToken:

Optional

lacework_proxyUrl:

lacework_aggregator:

lacework_aggregatorPort:

lacework_aggregatorDownloadCache:

lacework_aggregatorSensitiveDir:

lacework_autoUpgrade:

lacework_checkfreq:

lacework_dbSize:

lacework_aggregatorUrl:

lacework_aggregatorCert:

lacework_tags:

lacework_tokens:


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - hosts: localhost
      remote_user: root
      roles:
        - lacework_datacollector
      vars:
        - lacework_accessToken: "your token"

License
-------

