# mastodon-deploy
Deploy a glitchy but lovable microblogging server

### TL;DR

Go to `/deployment/inventory` and make a copy of all `*.yml.sample` files (remove the .sample extension) and insert your values/keys etc.

Review `/deployment/roles/create_containers/files/.env.prod` and change or add Mastodon specific configuration here. See ["Configuring your environment"](https://docs.joinmastodon.org/admin/config/) and [.env.production.sample](https://github.com/fedimix/mastodon/blob/main/.env.production.sample) for a list of all supported values.

To start the deployment:

```shell
cd deployment

ansible-playbook -i inventory/ playbooks/install.yml
```

Wait a couple of minutes ... done.

