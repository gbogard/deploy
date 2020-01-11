# Lambdacademy deployment


Pulling roles :

```
git submodule update --init --recursive
```

**Important** : installing hooks :

```
git config core.hooksPath ./git_hooks
```

Hooks ensure sensitive files will be encrypted by Ansible vault before being committed

Installing requirements :

```
ansible-galaxy role install -r roles/requirements.yml
```

## Vaults

- `secrets` (`./secrets`)

