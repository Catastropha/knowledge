# Supervisor

1 - install supervisor from ubuntu source

```apt install supervisor```

2 - create a config file

```echo_supervisord_conf > supervisord.conf```

3 - include other configs

```
[include]
files = /etc/supervisor/conf.d/*.conf
```

4 - copy supervisord.conf to the right place

```cp supervisord.conf /etc/supervisor/```

### Docker

Changes need to be done to run supervisor in docker

1 - turn daemon off so it can run in docker as main process (for docker)

```nodaemon=true```

2 - change CMD in Dockerfile to:

```CMD ["/usr/bin/supervisord"]```