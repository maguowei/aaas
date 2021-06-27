# aaas

Android as a service

```bash
# run Android emulator
$ docker run --name q-google-x86 -d --device /dev/kvm -p 8554:8554 -p 5555:5555 android4docker/q-google-x86:30.0.0

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

- [google/android-emulator-container-scripts](https://github.com/google/android-emulator-container-scripts
- [uiautomator2](https://github.com/openatx/uiautomator2) Android Uiautomator2 Python Wrapper
