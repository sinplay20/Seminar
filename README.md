# Pure Mathematics Seminar

这是一个不依赖构建工具的静态讨论班网页，用于展示和编辑：

- 学期名称、第一周起始日期、教学周总数，以及自动计算的当前教学周；
- Short Talk（周四 14:00–17:00）与 Long Talk（周五 14:00–16:00）的时间，以及每次报告可单独设置的地点；
- 可设置 Postdoc、PhD、Master 身份的成员，以及可增删、可编辑的 subgroup；
- Short Talk 的报告人、日期、类型与题目；新增记录会预填当前教学周的周四日期，但可以修改；
- Long Talk 的 selected paper、分组与连续报告安排；新增记录会预填当前教学周的周五日期，但可以修改；
- Lectures 学术报告记录，以及 Short Talk、Long Talk、Lectures 三个模块的本周汇总。

## 发布到 GitHub Pages

1. 在 GitHub 新建一个 repository。
2. 将压缩包中的 `index.html`、`.nojekyll` 和本文件上传到仓库根目录。
3. 打开仓库的 **Settings → Pages**。
4. 在 **Build and deployment** 中选择 **Deploy from a branch**。
5. 选择 `main` 分支和 `/(root)` 目录，然后保存。

几分钟后，GitHub 会在同一页面显示访问地址。

## 编辑说明

网页内的“学期设置”“编辑时间地点”“添加成员”“安排 Short Talk”“安排 Long Talk”和“记录 Lecture”按钮可以直接使用。修改内容保存在当前浏览器中；不同设备或不同成员之间不会自动同步。

若要永久修改公开网页中的默认内容，可在 `index.html` 中搜索 `const exampleData`，替换其中的示例成员、分组和报告安排，然后重新提交到 GitHub。
