# Sync Images

This is an example of a github action to pull automatically latest version of Falcon Sensor and Kubernetes Protection Agent (KPA).

**Configure secrets**

| Secrets to configure | Description |
| --- | --- |
| `FALCON_ART_USERNAME` | Login based on your CID to login to CrowdStrike registry |
| `FALCON_ART_PASSWORD` | Your password to connect to CrowdStrike registry |
| `FALCON_CLOUD_REGION` | Your assigned CrowdStrike Cloud region |
| `FALCON_KPA_DOCKER_USERNAME` | Login based on your CID to login to CrowdStrike registry |
| `FALCON_KPA_DOCKER_PASSWORD` | Your password to connect to CrowdStrike registry |
| `REGISTRY_HOST` | Your own registry FQDN (e.g. `registry.mycompany.com`) |
| `REGISTRY_USERNAME` | Your registry username |
| `REGISTRY_PASSWORD` | Your registry password |



**Configure the action**

If you want to configure the script behavior, here some parameters you can tune:
| Parameter | Description |
| --- | --- |
| `REGISTRY_REMOTE_REPO` | Default : `vendors/crowdstrike` |
| `NUMBER_OF_IMAGES_TO_TAKE_DAEMONSET` | Default value: `2` because x86 and aarch64 image|
| `NUMBER_OF_IMAGES_TO_TAKE_SIDECAR` | Default value: `1` |

