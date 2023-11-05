# qimg

Build `qcow2` image with grub installed from provided root-fs (e.g. from [dbs](https://kabr.metalica.space/rr/dbs)).

## synopsis

```sh
export QIMG_ROOTFS=/path/to/root-fs.tgz
export QIMG_IMAGE=/path/to/image.qcow2

require qimg [ /path/to/root-fs.tgz [ /path/to/image.qcow2 ] ]
```

## description

At least root-fs must be provided as source argument, in environment or as the command line argument. Command line arguments override environment variables. If the image name is not provided, `.tgz` is replaced by `.qcow2` and image will be in the same directory as the root-fs.
