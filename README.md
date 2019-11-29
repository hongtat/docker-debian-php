Custom PHP image built with hongtat79/base-debian and sury.org repo.

## Usage

To get started.

### docker

```
docker create \
  --name=php \
  --net=bridge \
  -v <path to php config>:/etc/php \
  -v <path to php run>:/run/php \
  --privileged
  --restart unless-stopped \
  hongtat79/debian-php
```

## Parameters


| Parameter | Function |
| :---- | --- |
| `-v /etc/php` | Location of PHP config files |
| `-v /run/php` | Location of PHP run files |
