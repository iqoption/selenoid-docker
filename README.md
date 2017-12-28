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

* [grid-router](https://github.com/iqoption/gridrouter-ansible)

grid-router may help you generate browser.xml (using sctl and ./files/input.json in grid-router repo).

#### Example

```yaml
---
- hosts: all
  roles:
  - selenoid
```

## Contributing
1. Fork it;
2. Create your feature branch: `git checkout -b my-new-feature`;
3. Commit your changes: `git commit -am 'Add some feature'`;
4. Push to the branch: `git push origin my-new-feature`;
5. Submit a pull request.

## License
See LICENSE
