# Tauri + Vue 3

This template should help get you started developing with Tauri + Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.


# Develop and Build

``` bash
# 安装依赖
npm install

# 本地运行
npm run dev

# 打包应用
npm run tauri build
```

打包报错：
* 运行桌面端的时候会从 github 上拉取依赖，可能会超时失败，可以直接换成 yarn 命令
* 命令行运行 rustup update，升级rustc版本，设置 rust 依赖国内镜像源
* WixTools、nsis 超时报错，自己手动下载下来，在电脑 %USERPROFILE%\AppData\Local\tauri (可直接复制，粘贴到电脑文件路径里会自动跳到这个目录)，目录下创建文件夹 NSIS 和 WixTools，将下载的压缩包内容解压至对应的文件夹下
* 自己看下 src-tauri/target 下面的打包文件，如果有生成其实就已经打包成功了

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)
