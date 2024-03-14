# meta-cmf-filogic
External layer for MediaTek filogic

### Quick Build steps

Follow this build steps to generate RDKB image and assuming that yocto environment setting is already done.
```
$ mkdir <workspace dir> 
$ cd <workspace dir> 

$ repo init -u https://code.rdkcentral.com/r/manifests -m rdkb-bpi-extsrc.xml -b hackathon2024/InfyTitans

$ repo sync -j4 --no-clone-bundle 
$ MACHINE=filogic830 source meta-cmf-filogic/setup-environment
$ bitbake rdk-generic-broadband-image
```
