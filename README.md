# Demo 网站压缩包说明

## 文件

- `LeanTTS_demo_website.zip`：可直接解压部署的 Demo 网站压缩包。
- 压缩包顶层目录为 `LeanTTS_demo/`。
- 包内只包含当前 `index.html` 实际引用的 128 条音频、网页文件和一份说明，不包含测试脚本、实验记录、历史指标及未被网页引用的旧音频。

## 解压与本地预览

```bash
cd /nfs/dataset-ofs-diar/luyuheng/lyh/edge/eval/zipvoice/top30_5models_comparison
unzip LeanTTS_demo_website.zip
python3 -m http.server 8765 --directory LeanTTS_demo
```

浏览器访问 `http://127.0.0.1:8765/index.html` 即可预览。

## 部署

将压缩包中的 `LeanTTS_demo/` 目录内容上传到 GitHub 仓库根目录，然后启用 GitHub Pages 即可。`index.html` 使用相对路径加载音频，不依赖服务器端程序。

