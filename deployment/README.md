
```shell
ansible-playbook -i inventory/ playbooks/install.yml
```

```shell
podman run --pod mstdn -ti --name ops \
    --env-file=/opt/config/.env.prod \
    europe-west3-docker.pkg.dev/txsvc-hq/txsvc-hq/mastodon:latest bin/tootctl accounts create ops --email ops@txs.vc --confirmed --role Owner

podman rm ops
```
