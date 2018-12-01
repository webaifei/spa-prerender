# prerender-spa-plugin example
> 单页应用 预渲染
## Project setup
```
// 设置临时环境变量跳过下载chromium
set PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=1
yarn install
```
### 手动下载chromium
1. 下载地址： https://download-chromium.appspot.com/ (需要翻墙)
2. 将下载的chromium 放到应用程序文件夹或者其他任意的文件夹下
3. 修改构建命令 (PUPPETEER_EXECUTABLE_PATH 就是你放置chromium的文件夹)
```
//package.json
{
  "build": "PUPPETEER_EXECUTABLE_PATH=/Applications/Chromium.app/Contents/MacOS/Chromium vue-cli-service build"
}
```
### Compiles and hot-reloads for development
```
yarn run serve
```

### Compiles and minifies for production
```
yarn run build
```

### Run your tests
```
yarn run test
```

### Lints and fixes files
```
yarn run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
