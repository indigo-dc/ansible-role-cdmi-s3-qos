CDMI S3 QoS Role
=========

Installs cdmi-s3-qos module for INDIGO developed CDMI server.

Role Variables
--------------

- `deb_get_url` (required in case of Ubuntu platform): URL to binary deb package with cdmi-s3-qos module and "embedded" CDMI server
- `deb_rpm_url` (required in case of CentOS platform): URL to binary rpm package with cdmi-s3-qos module and "embedded" CDMI server


Example Playbook
----------------

This is an example playbook of how to use CDMI S3 QoS role:

    - hosts: servers
      roles:
         - { role: indigo-dc.cdmi-s3-qos }

License
-------

Apache Licence v2
