# prettier

An opinionated code formatter based on Docker.

This is [prettier](https://github.com/prettier/prettier) wrapper.

## Requirements

- [Docker](https://www.docker.com/)

## Usage

### Format markdown

```shell
docker run --rm -v "$PWD:/work" unohealth/prettier-please --parser=markdown --write '**/*.md'
```

### Format json

```shell
docker run --rm -v "$PWD:/work" unohealth/prettier-please --parser=json --write '**/*.json'
```

### Help

```shell
docker run --rm unohealth/prettier-please
```

## Makefile targets

```text
build                          Build docker image
format                         Format
help                           Show help
install                        Install requirements
lint                           Lint
```

## Development

### Installation

```shell
git clone git@github.com:mmarell/prettier.git
cd prettier
make install
```

### Deployment

Automatically deployed by "[DockerHub Automated Build](https://docs.docker.com/docker-hub/builds/)" after merge.

### Deployment Pipeline

1. GitHub - Version Control System
   - <https://github.com/tmknom/prettier>
2. CircleCI - Continuous Integration
   - <https://circleci.com/gh/tmknom/prettier>
3. Docker Hub - Docker Registry
   - <https://hub.docker.com/r/tmknom/prettier/>
4. MicroBadger - Docker Inspection
   - <https://microbadger.com/images/tmknom/prettier>

## License

Apache 2 Licensed. See LICENSE for full details.
