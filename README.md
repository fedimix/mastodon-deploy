# mastodon-deploy
Deploy a glitchy but lovable microblogging server

### TL;DT

Go to `/deployment/inventory` and make a copy of all `*.yml.sample` files and insert your values/keys etc.

```shell
cd deployment

ansible-playbook -i inventory/ playbooks/install.yml
```

Wait a couple of minutes ... done.
