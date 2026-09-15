# English Notebook 网页版

这是预先构建的静态网页，不需要安装程序、Node.js 或服务器。

## 一次性发布
1. GitHub 创建公开仓库 english-coach。此仓库只放本网页程序，不能放学习备份、令牌或密码。
2. 解压网页包，进入 EnglishNotebook-Web 文件夹。用仓库的 Add file → Upload files 上传里面所有内容，包含 index.html、assets 文件夹、.nojekyll 和说明文件。不要上传 ZIP 本身，也不要再套一层 EnglishNotebook-Web 文件夹。
3. Settings → Pages → Source 选择 Deploy from a branch；Branch 选择 main，目录 /(root)，Save。
4. 等待 GitHub 显示发布成功，从 Pages 页面打开实际网址。预期网址是 https://jiangyimin123456.github.io/english-coach/，但该地址只有完成发布后才生效。

官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 首次连接同步
1. 再创建一个私有仓库 english-coach-data，添加 README。它专门存学习记录，不要设成公开，也不要对其启用 Pages。
2. 创建 Fine-grained personal access token，仅选择 english-coach-data，授予 Contents: Read and write。不要授权公开网页仓库。
3. 在网页的 GitHub 同步面板里输入令牌，设置同步解锁密码。令牌只发送给 GitHub，并加密保存在当前浏览器。不要将它上传到网页仓库或发送到聊天中。
4. 每台电脑分别配置一次，以后打开同一个网址并解锁，页面会自动同步。关闭网页后不同步。冲突会显示双方版本供选择。

## 使用与限制
- 不使用 ChatGPT 登录，不需要下载程序或购买服务器。首次打开网页仍需要网络。
- 本机数据保存在当前浏览器。请使用固定浏览器和相同网址，不要使用无痕模式或清除本站数据。
- 以前 localhost 本地版的数据不会自动出现在 GitHub Pages 新网址中；如已有数据，需先通过同一私有仓库同步，或导出导入一次备份。
- 学习记录上传到私有仓库但未额外加密；令牌和解锁密码不上传。账号及仓库访问权限由你管理。
- GitHub API 不可达时保留本机记录并重试；能访问 GitHub 首页并不保证 Pages 或 API 可达。
- 当前同步文件限制 850 KB，包含编辑历史；达到限制会停止云端上传并保留本机数据，届时需要升级同步方案。
- 收纳、手动学习、复习、设备朗读及文字回答保存可用，AI 模型尚未接入。
- 验证：TypeScript、构建、隔离浏览器的 GitHub Pages 子目录页面和模拟 GitHub 同步测试。真实仓库授权及跨电脑网络同步需连接后确认。
