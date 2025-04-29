# CordovaDocker
Repo hosting a docker image for Cordova.

Sample usage

```bash
git clone https://github.com/alexjyong/babbypaint.git
cd babbypaint
docker run --rm -i -v $PWD:/workspace -w /workspace --privileged ghcr.io/alexjyong/CordovaDocker:main sh -c "
        cd src &&
        cordova platform add android --verbose &&
        cordova plugin add cordova-plugin-x-toast &&
        cordova plugin add cordova-plugin-screen-pinning --verbose &&
        cordova build --verbose"
```
