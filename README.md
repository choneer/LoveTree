# LoveTree

基于 [AJLoveChina/LoveTree](https://github.com/AJLoveChina/LoveTree) 二次开发的爱情树网页，新增了可视化配置编辑器和动画速度控制功能。

## 功能

- Canvas 爱情树动画（种子生长 → 树枝延伸 → 花朵绽放）
- 打字机效果逐行显示情话
- 实时恋爱计时器
- 背景音乐（可开关）
- 树动画速度和文字速度独立配置
- 可视化配置编辑器（`/admin.html`），编辑后生成 config.js 下载部署

## 快速开始

### 直接使用

1. 修改 `config.js` 中的配置（情话、时间、名字等）
2. 部署到 GitHub Pages 或任意静态服务器

### 使用配置编辑器

1. 访问 `admin.html`
2. 编辑情话、相爱时间、双方名字、BGM 开关、动画速度
3. 点击「生成并下载 config.js」
4. 用下载的文件替换项目中的 `config.js`
5. 重新部署

## config.js 说明

```javascript
var config = {
    // 情话列表，每条一行，数量不限
    lines: [
        "亲爱的雯雯",
        "花开一季，有落红为证",
        "爱你永远。。。",
    ],
    // 相爱时间，格式: 年-月-日T时:分:秒
    date: "2017-07-20T20:15:00",
    // 双方的名字
    names: ["笨笨熊", "黑猪猪"],
    // 是否开启背景音乐
    bgm: true,
    // 树动画速度倍率（越大越慢，1=默认，0.5=快两倍，2=慢两倍）
    treeSpeed: 1,
    // 文字打字机速度倍率（越大越慢，1=默认）
    textSpeed: 1,
}
```

## 更换背景音乐

把你的音乐文件命名为 `music.mp3`，替换 `index_files/music.mp3` 即可。

## 致谢

- 原项目: [AJLoveChina/LoveTree](https://github.com/AJLoveChina/LoveTree)
- 作者: 霸都丶傲天
