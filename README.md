# aaas

Android as a service

```bash
# run Android emulator
$ docker run -d --device /dev/kvm --publish 8554:8554/tcp --publish 5555:5555/tcp android4docker/q-google-x86:30.0.0

# find device
$ adb kill-server
$ adb devices

# install uiautomator2
$ pipenv install uiautomator2
$ pipenv shell
$ uiautomator2 init

# open browser: <device_ip>:7912
```

## Ref

- [uiautomator2](https://github.com/openatx/uiautomator2) Android Uiautomator2 Python Wrapper
