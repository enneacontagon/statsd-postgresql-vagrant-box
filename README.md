# Graphite, Carbon, Grafana (2.x), PostgreSQL and StatsD

A vagrant/ansible configuration for testing postgresql integration with statsd

## Summary:

Provisions a virtual machine with vagrant containing

* Graphite (http://graphite.wikidot.com/)
* Carbon (http://graphite.wikidot.com/carbon)
* Grafana (2.x) (http://grafana.org/)
* PostgreSQL
* StatsD

## Details:

## Port overview
* Graphite: http://localhost:1080/
* Carbon: http://localhost:2003
* Grafana: http://localhost:1080/grafana/
* StatsD: 8125

## Installation

```
git clone https://github.com/enneacontagon/statsd-postgresql-vagrant-box.git
cd statsd-postgresql-vagrant-box
vagrant up
```

## Inspiration

Most of this is taken from https://github.com/pellepelster/graphite-grafana-vagrant-box
see LICENSE.pellepelster

statsd.yml, statsd.Debian.j2 and local_config.js.j2 were taken from https://github.com/dmichel1/ansible-statsd 
see LICENSE.dmichel1

postgresql.yml was derived from https://github.com/gulcin/2ndQuadrantBlog/tree/master/AnsibleLovesPostgreSQL
which has no LICENSE file
