## Notes

- all static files should be added to `root/static` then call it from anywhere as
`static/my-file`

- `.env` doesnt work, add environment variables directly to either `config/dev.env` or `config/prod.env`

- `cordova run android` auto runs after `yarn build`

- to save dev build to disk instead of memory use
```js
// before
"dev": "webpack-dev-server --inline --progress --config build/webpack.dev.conf.js"

// after
"dev": "webpack --watch --progress --config build/webpack.dev.conf.js"
```

## Read More

- https://cordova.apache.org/docs/en/latest/guide/platforms/android/
- https://cordova.apache.org/docs/en/latest/guide/next/#chrome-remote-debugging
- https://stackoverflow.com/questions/23204202/local-video-files-wont-play-in-cordova-android-app/36086827#36086827
- https://github.com/dpa99c/cordova-diagnostic-plugin
