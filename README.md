CDMI S3 QoS Role
=========

Installs and configure cdmi-s3-qos module together with embedded CDMI server.

Role Variables
--------------

- `deb_get_url` (required in case of Ubuntu platform): URL to binary deb package with cdmi-s3-qos module and "embedded" CDMI server
- `deb_rpm_url` (required in case of CentOS platform): URL to binary rpm package with cdmi-s3-qos module and "embedded" CDMI server
- `cdmi_port` (default: 8888): TCP port to which CDMI server is to bind
- `active_profile` (default: redis-embedded): possible values are "redis", "redis-embedded"



Example Playbook
----------------

This is an example playbook of how to use CDMI S3 QoS role:

    - hosts: servers
      roles:
         - { role: indigo-dc.cdmi-s3-qos, cdmi_port: 8080, active_profile: "redis-embedded" }

License
-------

Apache Licence v2
