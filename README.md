# VDDK Init

Simple repo to build the VDDK Init Image.

## Prerequisite

Create a Broadcom account and download 8.0.1 and untar it.

```shell
tar -xzf VMware-vix-disklib-<version>.x86_64.tar.gz
```

## Build and Push

Legally don't put this publicly out on the internet.

```shell
podman build . -t <registry_route_or_server_path>/vddk:<tag>
podman push <registry_route_or_server_path>/vddk:<tag>
```

## References

1. [OpenShift Docs](https://docs.redhat.com/en/documentation/migration_toolkit_for_virtualization/2.7/html/installing_and_using_the_migration_toolkit_for_virtualization/prerequisites_mtv#creating-vddk-image_mtv)
2. [Broadcom Download Page](https://developer.vmware.com/web/sdk/8.0/vddk)
