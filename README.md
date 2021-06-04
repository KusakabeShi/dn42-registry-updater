# dn42-registry-updater
The github action of this repo will automatically pull everything from https://git.dn42.dev/dn42/registry and push to https://github.com/KusakabeSi/dn42-registry

To reduce the server load of git.dn42.dev, This is what I do:

1. Clone from git@github.com:KusakabeSi/dn42-registry.git
2. Change origin to git@git.dn42.dev:dn42/registry.git
3. Pull from git.dn42.dev. In most time, it will only get ```Already up to date.```, so it will not cosume too many network traffic.
4. Change back to github.com and git push
