## Selenoid in docker
[![Build Status](https://travis-ci.org/iqoption/selenoid-docker.svg?branch=add-travis)](https://travis-ci.org/iqoption/selenoid-docker)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Set up [selenoid](https://github.com/aerokube/selenoid) in docker

#### Requirements

* `python`
* `docker`

#### Variables

* `selenoid_cm_version`: [Default: `1.3.1`] Install configuration manager version
* `selenoid_version`: [Default: `1.4.0`] Install selenoid version
* `selenoid_docker_api_version`: [Default: `1.24`] Docker api version (for Selenoid)
* `selenoid_limit`: [Default: `4`] Total number of simultaneously running containers ([full docs](http://aerokube.com/selenoid/latest/#_recommended_docker_settings))
* `selenoid_tmpfs`: [Default: `128`] Add in-memory filesystem (tmpfs) to container ([full docs](http://aerokube.com/selenoid/latest/#_other_optional_fields))
* `selenoid_config_dir`: [Default: `/etc/selenoid`] Selenoid configuration dir
* `selenoid_listen_port`: [Default: `4444`] Listen port
* `selenoid_time_zone`: [Default: `Europe/Moscow`] Timezone in container

#### Example

```yaml
---
- hosts: all
  roles:
  - selenoid
```

## Dependencies

* [grid-router](https://github.com/iqoption/gridrouter-ansible)

grid-router may help you generate browser.xml (using sctl and ./files/input.json in grid-router repo).

## Contributing
1. Fork it;
2. Create your feature branch: `git checkout -b my-new-feature`;
3. Commit your changes: `git commit -am 'Add some feature'`;
4. Push to the branch: `git push origin my-new-feature`;
5. Submit a pull request.

## License
See LICENSE
