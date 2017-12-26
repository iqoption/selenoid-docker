## Selenoid in docker

Set up [selenoid](https://github.com/aerokube/selenoid) in docker

#### Requirements

* `python`
* `docker`

#### Variables

* `selenoid_cm_version`: [Default: `1.3.1`] Install configuration manager version
* `selenoid_version`: [Default: `1.4.0`] Install selenoid version
* `selenoid_docker_api_version`: [Default: `1.24`] Docker api version (for Selenoid)

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - selenoid
```
