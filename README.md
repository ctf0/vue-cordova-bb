- all static files should be added to `root/static` then call it from anywhere as
`static/my-file`

- `cordova run android` auto runs after `yarn build`

- to save dev build to disk instead of memory use
```js
// before
"dev": "webpack-dev-server --inline --progress --config build/webpack.dev.conf.js"

// after
"dev": "webpack --watch --progress --config build/webpack.dev.conf.js"
```

- check
  + https://cordova.apache.org/docs/en/latest/guide/platforms/android/
  + https://cordova.apache.org/docs/en/latest/guide/next/#chrome-remote-debugging
  + https://stackoverflow.com/questions/23204202/local-video-files-wont-play-in-cordova-android-app/36086827#36086827
  + https://github.com/xjxxjx1017/cordova-phonegap-android-sdcard-full-external-storage-access-library
  + https://github.com/dpa99c/cordova-diagnostic-plugin
