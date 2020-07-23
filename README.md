Role Name
=========

Install the Lacework Datacollector Agent on systems using the yum or apt package manager.


Role Variables
--------------

***Required***

lacework_accessToken

***Optional***

lacework_proxyUrl\
lacework_aggregator\
lacework_aggregatorPort\
lacework_aggregatorDownloadCache\
lacework_aggregatorSensitiveDir\
lacework_autoUpgrade\
lacework_checkfreq\
lacework_dbSize\
lacework_aggregatorUrl\
lacework_aggregatorCert

lacework_tags (Dictionary)

Note: All lacework_tags values should be quoted. Booleans will not work unless they are quoted)


Example Playbook
----------------

    ---
    - hosts: lacework_servers
      become: yes
      roles:
        - lacework_datacollector
      vars:
        - lacework_accessToken: "your token"
        - lacework_tags:
            foo: bar
            # you must quote boolean tag values
            test: "true"

License
-------
Copyright 2020 Filippo Di Noto (xdfil)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
