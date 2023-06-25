# Dev Container Features: 

This repository contains a number of common devcontainer features that I needed to be productive.

## Features

### `postgresql-client`

This layer will install the postgres at the major version specified by the `version` property.

```jsonc
{
    "image": "mcr.microsoft.com/devcontainers/base:ubuntu",
    "features": {
        "ghcr.io/robbert229/devcontainers-features/postgresql-client:1": {
            "version":"14"
        }
    }
}
```

```bash
psql --version
```
