# 唐可儿 · 个人品牌网站

纯静态页面：原生 HTML + CSS + 少量 JavaScript，无框架、无构建步骤。

## 文件结构

```
个人品牌网站/
├── index.html          全部页面（内容、样式、交互都在这一个文件里）
├── assets/
│   └── portrait.jpg    形象照（首屏右栏）
├── 网站定位卡-v2.md     定位与事实来源清单
└── 版式笔记-参考站.md    版式依据
```

## 一、在电脑上预览（不需要装任何东西）

**方法 1：直接双击 `index.html`**，用浏览器打开即可。页面不依赖任何本地服务。

**方法 2（更接近真实效果，可选）**：在文件夹地址栏输入 `cmd` 回车，然后执行：

```
python -m http.server 8000
```

浏览器打开 `http://localhost:8000`。（需要电脑装有 Python；没有就用方法 1，效果一样。）

> 提示：按 F12 打开开发者工具，点左上角的手机图标，可以模拟手机宽度查看。

## 二、发布到 GitHub Pages（网页操作，不用命令行）

1. 登录 [github.com](https://github.com)，右上角 **+ → New repository**
2. Repository name 随意（如 `portfolio`），选 **Public**，点 **Create repository**
3. 在仓库页点 **uploading an existing file**（或 Add file → Upload files）
4. 把 `index.html` 和 `assets` 文件夹（含 `portrait.jpg`）拖进去，点 **Commit changes**
5. 进 **Settings → Pages**，在 Branch 下选 `main` + `/ (root)`，点 **Save**
6. 等一两分钟，页面顶部会出现网址：`https://你的用户名.github.io/portfolio/`

以后改内容：重新上传 `index.html` 覆盖即可，一分钟内生效。

> 注意：从你当前的网络访问 github.com 有时需要开代理。如果打不开或上传失败，开代理再试；或者用 **Netlify Drop**（https://app.netlify.com/drop ，把整个文件夹拖进去即上线，免注册版链接 24 小时有效，注册后永久）作为备选。

## 三、换照片 / 改内容

- **换照片**：把新照片命名为 `portrait.jpg`，覆盖 `assets/portrait.jpg` 即可。竖版 2:3 比例效果最好（现在的照片是 1280×1920）。
- **改文字**：用记事本或 VS Code 打开 `index.html`，直接搜文字改。所有数字和经历都有出处，改之前对照《网站定位卡-v2.md》里的事实来源清单。
- **字体说明**：页面用 Google Fonts 加载「思源宋体」，访客第一次打开会从网络加载；断网时会自动退回系统宋体，页面不会坏。

## 四、待确认事项（上线前过一遍）

见《网站定位卡-v2.md》末尾：
1. 「连续 4 个年度」的口径
2. 平台名要不要从「头部心理咨询平台」换成实名「壹心理」
3. 电话要不要上站（现在只有邮箱）
4. 公司业绩数据是否允许公开
