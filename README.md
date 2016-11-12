docker-alpine-bloomd
-------------------------
Alpine-base docker image for [bloomd](https://github.com/armon/bloomd).

Usage

```shell
docker run -p 8673:8673 \
           -v /path/to/data:/data \
           steranin/bloomd
```

If you need to customize bloomd's configuration you can mount the folder containing bloomd.conf at `/etc/bloomd/` 

```shell
docker run -p 8673:8673 \
           -v /path/to/db:/db \
           -v /path/to/etc/bloomd:/etc/bloomd \
           steranin/bloomd 
```
