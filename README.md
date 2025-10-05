# diabsurance

Homepage created end of June 2025.
Covers the insurance broker activities.
Diabsurance is short for diabetes+insurance.

# Deployment
Uses GIThub pages

This is still WIP.

## Dev Branch and 'diabsurance_dev' Repository
GIThub pages only builds one webpage per repository. (Screenshot)

Therefore the dev branch of the `diabsurance` repository is mirrored to `diabsurance_dev`
via 'git '.

For simplicity, please avoid modifications to `diabsurance_dev`. It is just to build a real live version of the webpage.
(For development there are different tools, such as Live Server. Still, BR found the possibility to publish the dev branch useful.)



## master and dev branch
master and dev branch have different CNAME-files:
diabsurance.de (master) and 
dev.diabsurance.de (dev)

The latter CNAME only plays out in the `diabsurance_dev` repository, while the CNAME of master is `diabsurance.de`.

`.gitattributes` plays a role as well as `.git\config`, which has been set according to this advice by chatGPT:
(Screenshot)

```
CNAME merge=ours    # .gitattributes
```

```
[merge "ours"]    # .git/config
    name = Keep our version during merge
    driver = true  
```
