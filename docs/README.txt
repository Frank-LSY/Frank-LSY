Shuyu Lu — static personal website
Exported: October 24, 2026
Source version: f665f9461ed676dcb91caeed8676a50b312dd236

部署说明
1. 解压 ZIP，将解压后的全部内容上传到静态网站托管服务的发布目录。
2. index.html 必须位于发布目录根目录；保留 assets、photos、posters 的相对位置。
3. 这是纯静态 HTML/CSS 网站，无需 npm、构建命令、服务器程序或数据库。
4. 本地查看可直接打开 index.html；外部项目、论文和社交链接需要联网。

GitHub Pages：将包内内容放入所选发布分支的根目录，并在仓库 Pages 设置中选择该分支和根目录。
其他静态托管：直接上传解压后的目录，使用 index.html 作为首页。

包含内容
- index.html、styles.css：可直接编辑的页面与样式
- cv.pdf：简历
- assets/：木纹背景素材
- photos/：头像与生活照片
- posters/：海报页面、预览和完整图片
- .nojekyll：便于原样发布到 GitHub Pages

隐私提醒
此包不包含原托管平台的登录保护。若部署到公开网址，页面、CV、照片和海报也将公开可访问。
包内不包含 Git 历史、访问凭据、平台配置或本地临时文件。

Static deployment notes
Upload the extracted files as-is. No build step is required. Keep index.html at
the publishing root and preserve the asset directory structure. Relative asset
links support deployment under a project subdirectory as well as a domain root.
This export has no authentication layer; use private hosting if access must be restricted.
