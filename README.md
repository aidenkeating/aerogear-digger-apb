# Buildfarm APB

## What does it do?
* Installs Android SDK pod into the project
* Creates an OpenShift Jenkins if it does not exist in a project
* Adds the android-signing plugin into the OpenShift Jenkins pod
* Creates the ConfigMap to configure the Jenkins Kubernetes Plugin

## Developing

After making your required changes, update the apb.yml to point at your own docker organisation, run:

```bash
make DOCKERORG=<your docker org> DOCKERHOST=<defaulting to docker.io>
```

## TODO
* Creates an OpenShift Jenkins if it does not exist in a project
* Adds the android-signing plugin into the OpenShift Jenkins pod (https://github.com/aidenkeating/mobile-next-jenkins)
* Creates the ConfigMap to configure the Jenkins Kubernetes Plugin (https://gist.github.com/aidenkeating/66e4ac393a81407b809fe993a7b2e1e3)
