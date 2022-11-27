## Practicus AI Container Registry

Please visit Practicus AI documentation at [https://docs.practicus.ai](https://docs.practicus.ai) to learn how to deploy cloud containers locally or in the cloud.

### Explanation of tags 

- **yy.m.d** : Practicus AI cloud platform version tag (e.g. 22.11.0)
- **latest** : Production grade latest image
- **preview** : Nightly build image

### Selecting a version

- Please prefer to use the latest Practiucus AI app version together with the latest cloud platform.
- If this is not the case, please use matching versions between the app and cloud. 
- Matching **yy.m** version tags will be sufficient. 
  - App version 22.11.x will be compatible with the cloud version 22.11.y and vice versa
  - App version 22.12.x might **not** be compatible with cloud version 22.11.y

### Sample container pull commands

#### Pulling a particular version 
```shell
docker pull ghcr.io/practicusai/practicus:22.11.0
```

#### Freedom to choose a container engine
- In order to use a container engine other than docker, simply replace docker with the subject engine command
- We support and tested with Podman. Use others with caution

```shell
podman pull ghcr.io/practicusai/practicus:22.11.0
```

#### Pulling production image
```shell
docker pull ghcr.io/practicusai/practicus:latest
```

#### Pulling nighlyt build image
```shell
docker pull ghcr.io/practicusai/practicus:preview
```
