# 协作约定

## 1. 分支

- `main`：随时能跑的主线。**不要直接往 main 推代码。**
- 做新功能或修 bug 时，新建自己的分支，命名：
  - `feat/功能名`　例：`feat/random-picker`、`feat/canteen-list`
  - `fix/问题名`　 例：`fix/login-error`
  - `docs/文档名`　例：`docs/readme`

## 2. 提交信息（commit message）

格式：`类型: 简短说明`

类型：`feat` 新功能 / `fix` 修 bug / `docs` 文档 / `refactor` 重构 /
`style` 格式（不改逻辑）/ `chore` 杂项

例子：
- `feat: 新增食堂列表页`
- `fix: 修复随机推荐结果重复`
- `docs: 补充本地运行说明`

**一次提交只做一件事**，不要把"改页面 + 修 bug + 加图片"混在一起。

## 3. 合并流程

1. 开工前先拉取最新的 main
2. 在自己的分支上开发
3. 写完推送分支，开 Pull Request（PR）合并到 main
4. 至少找 1 个人看过再合并
5. 合并后删掉自己的分支

> ⚠️ 组织内仓库均为 Free 方案的私有仓库，GitHub 无法强制上述规则，
> main 分支任何人都能直接推送。以上流程**全靠自觉**，请务必遵守。

## 4. 不要提交的东西

- `.env`、密钥、密码、token、账号
- 编译产物、系统临时文件
- 大文件（视频、上百 MB 的图片） 素材文件请使用其他方式同步 不要上传至仓库

## 5. 每个人用自己的 GitHub 账号提交

不要共用账号。

## 6. 遇到冲突

- 动手前先拉取最新代码，能避免大部分冲突
- 真的冲突了：**谁的分支谁解决**；解决不了就在群里喊人，
  不要直接删掉别人的代码

## 7. 常用命令（或者直接使用桌面端）

```bash
git pull                      # 开工前拉最新
git checkout -b feat/xxx      # 新建并切到自己的分支
git add .                     # 暂存改动
git commit -m "feat: xxx"     # 提交
git push -u origin feat/xxx   # 推送分支
