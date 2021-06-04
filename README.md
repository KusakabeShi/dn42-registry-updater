# dn42-registry-updater
The github action of this repo will automatically pull everything from https://git.dn42.dev/dn42/registry and push to https://github.com/KusakabeSi/dn42-registry

To reduce the server load of git.dn42.dev, This is what I do:

1. Clone from git@github.com:KusakabeSi/dn42-registry.git
2. Change origin to git@git.dn42.dev:dn42/registry.git
3. Pull from git.dn42.dev. 
    * It already contains old files comes from step one to prevent download whole repo.
    * So it won't cosume too many network traffic and cpu loading of git.dn42.dev.
5. Change origin back to github.com and git push.
