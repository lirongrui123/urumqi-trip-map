# 乌鲁木齐 · 4天半4晚行程地图

静态网页，包含按天切换的行程、路线示意、地理地图和手绘原图。住宿为全季酒店（乌鲁木齐友好店）。

## GitHub Pages 发布

建议仓库名：`urumqi-trip-map`。网站不需要构建命令、Node.js 或 API Key。

1. 将本文件夹里的文件放在仓库根目录，确保根目录有 `index.html`。
2. 在仓库的 **Settings → Pages → Build and deployment** 中，Source 选择 **Deploy from a branch**。
3. Branch 选择 **main**，目录选择 **/(root)**，点击 **Save**。
4. 等待 Pages 部署成功，以该页面实际返回的网站链接为准。

配置完成后，更新 main 分支中的网站文件即可触发重新发布。当前文件包已就绪，但还未上传到 GitHub，也未启用 Pages。

GitHub Free 通常使用公开仓库来启用 Pages；Pages 网页通常公开可访问，原 ChatGPT 网站的登录限制不会随这些静态文件迁移。请以账号和组织的实际设置为准。

官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 文件

- `index.html`：入口页面。
- `app.js`：行程数据和交互逻辑。
- `style.css`：页面样式和手机适配。
- `leaflet.js`、`leaflet.css`：本地地图组件。
- `route-plan.jpg`：用户上传的手绘路线图。
- `.nojekyll`：以原始静态文件发布。

所有本地资源采用相对路径，可用于 GitHub Pages 的项目子路径。

## 地图说明

路线示意和行程内容随文件提供；地理底图使用联网的 CARTO / OpenStreetMap 服务，地图搜索会跳转高德或 Apple 地图。GitHub Pages 与底图服务的国内访问效果尚未实测。

酒店坐标仍为商圈参考位置；沙沟入口、航班和票务待核对事项保持原样。
