It seems `expo-router` listens for any schemes/url.
This is an issue if you want to open `content:` schemes for instance.

```bash
npm i 
```

Build the development app. You can run:

```bash
npm run build
adb push ./test.txt /sdcard/Download
adb push ./build-xxx.apk /sdcard/Download
```

Install the apk from the phone/emulator, then open `test.txt` from a file manager with the development app.

You will be redirected to a non existing screen.
Instead, I would expect being able to catch the `content:` url to handle the file programmatically.

