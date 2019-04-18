# phare

This repo provisions and configures a monitoring and alerting
solution for the TVB INS platform.  To avoid outage problems akin
to S3-status-hosted-on-S3 comedy AWS has put on, this is built on
an alternative stack

- GitHub for code
- Travis for builds
- Google Cloud for running the VM
- MessageBird for sending SMS

Ansible is used to provision the VM, configure it, update the
DNS records, update/backup the data.

This VM should host

- [ ] Prometheus
- [ ] Alertmanager
- [ ] Grafana
- [ ] Periodic backups of monitoring data
- [ ] Rocketchat for out of band team communication
