# s3cmd

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/s3cmd)
[![General Workflow](https://github.com/rolehippie/s3cmd/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/s3cmd/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/s3cmd/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/s3cmd/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/s3cmd/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/s3cmd/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/s3cmd)](https://github.com/rolehippie/s3cmd/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.s3cmd-blue)](https://galaxy.ansible.com/rolehippie/s3cmd)

Ansible role to install and configure S3 command-line client.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Default Variables](#default-variables)
  - [s3cmd_access_key](#s3cmd_access_key)
  - [s3cmd_bucket_location](#s3cmd_bucket_location)
  - [s3cmd_host_base](#s3cmd_host_base)
  - [s3cmd_host_bucket](#s3cmd_host_bucket)
  - [s3cmd_secret_key](#s3cmd_secret_key)
  - [s3cmd_users](#s3cmd_users)
  - [s3cmd_version](#s3cmd_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### s3cmd_access_key

Access key for connection

#### Default value

```YAML
s3cmd_access_key:
```

### s3cmd_bucket_location

Bucket location for connection

#### Default value

```YAML
s3cmd_bucket_location: us-east-1
```

### s3cmd_host_base

Host base for connection

#### Default value

```YAML
s3cmd_host_base:
```

#### Example usage

```YAML
s3cmd_host_base: storage.example.com
```

### s3cmd_host_bucket

Host bucket for connection

#### Default value

```YAML
s3cmd_host_bucket: '{{ s3cmd_host_base }}/%(bucket)'
```

### s3cmd_secret_key

Secret key for connection

#### Default value

```YAML
s3cmd_secret_key:
```

### s3cmd_users

#### Default value

```YAML
s3cmd_users: []
```

### s3cmd_version

Define a specific version to install

#### Default value

```YAML
s3cmd_version:
```

## Discovered Tags

**_s3cmd_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
