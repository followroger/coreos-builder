# CoreOS in Docker

## Start
```
./coreos-builder 1409.8.0
cd coreos
docker build -t followroger/coreos .
docker run --privileged --rm -it followroger/coreos
```

## Notes

Provide `/var/lib/coreos-install/user_data`, `/usr/share/oem/cloud-config.yml`, and `/usr/share/oem/bin/setup-environment` to configure the container accordingly.

Follow guides at https://coreos.com.
