# 今晚唱什么

单设备抽歌转盘。GitHub Pages 可直接托管仓库根目录的 `index.html`。

- 普通歌单按行导入，不需要密钥。
- 杂乱文字或图片可在页面临时填写 DeepSeek API Key，调用官方 `deepseek-flash` Chat Completions 视觉接口，再人工核对。
- Key 仅在页面内存里，不保存在 localStorage。歌单和抽取进度保存于本机 localStorage。
- 每次从剩余项随机选取，动画完成后加入抽取历史，不会重复。

注意：静态网页的浏览器直连 API 取决于 DeepSeek 是否允许该来源的 CORS 请求。若浏览器阻止跨域请求，需要加入受控代理；不要将共享 API Key 放在公开仓库或网页源代码里。
