## Selenoid in docker
[![Build Status](https://travis-ci.org/iqoption/selenoid-docker.svg?branch=add-travis)](https://travis-ci.org/iqoption/selenoid-docker)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Set up [selenoid](https://github.com/aerokube/selenoid) in docker

#### Requirements

* `python`
* `docker`

#### Variables

```yaml
selenoid_version: 1.6.0
selenoid_cm_version: 1.4.2
selenoid_limit: 5
selenoid_tmpfs: 128
selenoid_config_dir: /etc/selenoid
selenoid_listen_port: 4444
selenoid_time_zone: Europe/Moscow
selenoid_browsers_last_versions: 5
selenoid_browsers:
  - firefox
  - opera
  - chrome
selenoid_video_host_output_dir: /var/lib/selenoid/video
selenoid_video_container_output_dir: /opt/selenoid/video
```

#### Example

```yaml
---
- hosts: all
  roles:
  - selenoid
```

## Dependencies

* [grid-router](https://github.com/iqoption/gridrouter-ansible)

## Contributing
1. Fork it
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License
See LICENSE
