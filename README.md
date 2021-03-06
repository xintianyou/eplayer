<p align="center"><img src="http://ww1.sinaimg.cn/large/0065Zy9egy1fvcjfzaa1lj30dw0dwwhe.jpg" alt="eplayer logo" width="200px"></p>


# eplayer   [![NPM version](https://img.shields.io/npm/v/eplayer.svg?style=flat-square)](https://npmjs.com/package/eplayer) [![NPM downloads](https://img.shields.io/npm/dm/eplayer.svg?style=flat-square)](https://npmjs.com/package/eplayer)

:dart: A simple and lovely html5 video player

#### who use eplayer？

[epayer.js.org - 官网（demo）](https://eplayer.js.org/)

[clicli.us - C 站](https://www.clicli.us/)

### Install
```shell
yarn add eplayer -S
```

### Use

dom，这是一个 web-components 组件

```html
<e-player></e-player>
```
css，可选，用于穿透 shadow-dom 预留的默认样式，默认为蓝色
```css
e-player {
  /* 进度条底色 */
  --progress:rgba(255,255,255,.3);
  /* 进度条偏移颜色 */
  --buffer:#f2e;
  /* 按钮颜色 */
  --dot:#f2e;
  /* 图标颜色 */
  --icons:#fff
}
```

js，只需要 new 一个 Ep 类

```javascript
import Eplayer from 'eplayer'

new Eplayer({
  src: '001.mp4',
  type:'mp4'
})
```

if m3u8 need supported，please install `hls.js` first

```shell
npm i hls.js -S
```

#### development

```shell
yarn start
```

#### Screenshot

![free eplayer](https://ws1.sinaimg.cn/mw690/0065Zy9egy1fymn1nwo3ej30rq0fmtid.jpg)
