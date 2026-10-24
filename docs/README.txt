Shuyu Lu — static personal website / SEO edition
Exported: October 24, 2026
Base source version: f665f9461ed676dcb91caeed8676a50b312dd236, with SEO updates
Production URL: https://frank-lsy.github.io/Frank-LSY/

SEO 更新与 Search Console
- 已原样保留用户提供、且在线上核对过的 google-site-verification meta 标签。
- 主页标题更新为 Shuyu Lu | Clinical AI Research | UTHealth Houston。
- 优化简介，为主页和两张海报页面设置各自的 canonical 首选网址。
- 添加 ProfilePage / Person JSON-LD，关联 Scholar、LinkedIn 和 GitHub。
- 添加社交分享元数据；保留原有正文、布局、样式、CV 和照片。
- sitemap.xml 包含三个独立 HTML 页面，不把 #research 等锚点当成独立页面。
- 本包没有自动发布，上传并等待 GitHub Pages 部署完成后，在已有 Search Console
  资源的“站点地图 / Sitemaps”中提交：
  https://frank-lsy.github.io/Frank-LSY/sitemap.xml
- 再用“网址检查 / URL inspection”检查主页，测试实际网址后请求编入索引。
- 不要删除验证标签，Google 可能再次检查所有权。无需重新添加已验证的资源。
- 收录和排名不保证，结构化数据也不保证特殊搜索外观。

robots.txt 说明
未添加 /Frank-LSY/robots.txt，因为搜索引擎只使用主机根目录的
https://frank-lsy.github.io/robots.txt。项目目录内的 robots.txt 不控制抓取。
无需为此次更新新建根站点；直接在 Search Console 提交 sitemap 即可。
若根目录以后设置抓取限制，请确保未屏蔽 /Frank-LSY/。

维护说明
- 此包针对上述固定生产 URL 配置。迁移域名或路径时，同步更新 canonical、
  sitemap.xml、JSON-LD 和社交分享元数据中的绝对网址。
- Google 验证标签是公开的验证标识，不是访问密码。
- 原始导出包仍保留，可以恢复旧版本。

部署说明
1. 解压 ZIP，将解压后的全部内容上传到静态网站托管服务的发布目录。
2. index.html 必须位于发布目录根目录；保留 assets、photos、posters 的相对位置。
3. 这是纯静态 HTML/CSS 网站，无需 npm、构建命令、服务器程序或数据库。
4. 本地查看可直接打开 index.html；外部项目、论文和社交链接需要联网。

当前 GitHub Pages：将包内内容合并到 Frank-LSY/Frank-LSY 仓库的 docs/ 目录，
覆盖同名文件，保留其他仓库文件。应得到 docs/index.html 和 docs/sitemap.xml，
不要再嵌套一层文件夹。保持 Pages 现有发布设置不变。
其他静态托管：上传解压目录，使用 index.html 作为首页；更换网址须更新 SEO 绝对网址。

包含内容
- index.html、styles.css：可直接编辑的页面与样式
- cv.pdf：简历
- assets/：木纹背景素材
- photos/：头像与生活照片
- posters/：海报页面、预览和完整图片
- .nojekyll：便于原样发布到 GitHub Pages
- sitemap.xml：供 Search Console 提交的站点地图

隐私提醒
此包不包含原托管平台的登录保护。若部署到公开网址，页面、CV、照片和海报也将公开可访问。
包内不包含 Git 历史、访问凭据、平台配置或本地临时文件。

Static deployment notes
Upload the extracted files as-is. No build step is required. Keep index.html at
the publishing root and preserve the asset directory structure. Relative asset
links support deployment under a project subdirectory as well as a domain root.
This export has no authentication layer; use private hosting if access must be restricted.
For the current GitHub repository, merge the archive contents into docs/ and
preserve unrelated files. The verification meta tag is retained. After deployment,
submit the sitemap URL above in the existing Search Console property and inspect
the homepage. Canonical, JSON-LD, sitemap and social URLs target the production
URL above; update these if you move the site. This ZIP does not publish changes.
