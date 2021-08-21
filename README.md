# Prometheus Grafana and Elasticsearch stack
## Only for local tests, because ssl/tls not enabled for this test environment
Before starting, you need to install docker and docker-compose.
1. Add to ***etc/hosts***
```bash
<your IP> alertmanager.monitoring.int
<your IP> cadvisor.monitoring.int
<your IP> efk.monitoring.int
<your IP> grafana.monitoring.int
<your IP> prometheus.monitoring.int
```
2. Set for grafana directory permissons for full access
```bash
chmod 777 -R grafana/
```
3. Run docker compose
```bash
docker-compose up -d
```
4. Login and password for all access
```
login:    admin
password: Pometheus
```
5. Change IP's in ***./prometheus/sd_test.json*** for discovery from file.
