# Minimal WordPress MySQL Pod

Just a playground.

![Screenshot](screenshot.png)

## Run pod

```
podman play kube pod.yaml
```

## Play around with WordPress

[http://localhost:8080/](http://localhost:8080/)

## Restart pod

```
podman pod restart mwmp
```

***#FIXME*** You may need to restart the pod a second time if you previously stopped the container:
```
podman pod restart mwmp
```

## Remove pod and volumes

```
podman pod rm -f mwmp
podman volume rm mwmp-mysql-volume mwmp-wordpress-volume
```