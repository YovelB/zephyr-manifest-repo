## minimal T3 topology manifest repo for zephyr

## quick start

```bash
# on arch
sudo pacman -Syu

# install depdendencies
sudo pacman -S git cmake ninja gperf ccache dfu-util dtc wget \
    python-pip python-setuptools python-wheel tk xz file make

# initialize west workspace with this manifest
west init -m https://github.com/YovelB/zephyr-manifest-repo [workspace-name]

# enter the workspace
cd zephyr-workspace

# fetch all the required modules
west update

# export zephyr environment variables
west zephyr-export

# install python dependencies
west packages pip --install

# (optional) install zephyr sdk using west or manually
```

## notes

- up-to-date documentation - [zephyr offical docs](https://docs.zephyrproject.org/latest/index.html)
