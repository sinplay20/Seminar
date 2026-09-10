# Pure Mathematics Seminar

这是一个可直接发布到 GitHub Pages 的静态讨论班网站。项目分为三个部分：

- `index.html`：课题组成员访问的公开只读页面；
- `admin.html`：管理员编辑页面，修改先保存为当前浏览器中的草稿；
- `data/seminar.json`：GitHub Pages 实际展示的正式排期数据。

公开页面包含 Short Talks、Long Talks、Lectures、本周学术活动总览、subgroup 和成员信息。Short Talk 默认为周四 14:00–17:00，Long Talk 默认为周五 14:00–16:00；新增场次的日期会根据学期第一周自动预填，之后仍可修改。

## 第一次发布到 GitHub Pages

1. 在 GitHub 新建一个 repository，例如 `pure-math-seminar`。
2. 解压源码包，将其中所有文件和文件夹上传到仓库根目录。必须保留 `data/seminar.json` 的目录结构。
3. 打开仓库的 **Settings → Pages**。
4. 在 **Build and deployment** 中选择 **Deploy from a branch**。
5. 选择 `main` 分支和 `/(root)`，点击 **Save**。
6. 等待 GitHub 完成发布。公开地址通常为：

   `https://你的用户名.github.io/仓库名/`

管理员页面地址为：

   `https://你的用户名.github.io/仓库名/admin.html`

建议把管理员页面加入浏览器书签，不必把它发给组员。

## 每次修改排期

1. 登录 GitHub，然后打开 `admin.html`。
2. 使用页面中的“学期设置”“安排 Short Talk”“安排 Long Talk”“记录 Lecture”等按钮编辑。
3. 每次点击保存，修改只进入当前浏览器的本机草稿，尚未公开。
4. 检查无误后点击 **复制 JSON**。
5. 回到 GitHub 仓库，打开 `data/seminar.json`，点击右上角铅笔按钮。
6. 全选旧内容，粘贴新的 JSON，点击 **Commit changes**。
7. GitHub Pages 自动更新后，组员刷新公开页面即可看到新排期。

也可以点击 **导出 seminar.json**，然后进入仓库的 `data` 文件夹，选择 **Add file → Upload files**，上传同名文件并提交。

## 管理员权限

真正的发布权限由 GitHub 仓库控制，而不是由 `admin.html` 控制。即使其他人知道管理员页面地址，他们的修改也只会保存在自己的浏览器中，无法改动正式排期。

- 在 **Settings → Collaborators** 中，只给确实需要发布排期的人写入权限。
- 普通组员只需要访问 GitHub Pages，不需要加入仓库。
- 不要在网页源码中写入 GitHub Personal Access Token、密码或其他密钥。
- 公开页面中的 `seminar.json` 也是公开数据，不要填写不适合公开的个人信息。

## 草稿与恢复

- **恢复本机草稿**：重新载入当前浏览器里尚未发布的修改。
- **重新载入已发布数据**：重新读取仓库中的 `data/seminar.json`。
- **恢复示例数据**：用源码自带的示例覆盖当前本机草稿，不会直接修改 GitHub。

如果换电脑管理排期，新设备不会自动获得旧设备的本机草稿，但始终可以从 GitHub 载入最近一次正式发布的数据。
