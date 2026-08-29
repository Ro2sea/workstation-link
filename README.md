# 沅的综合工作台 · 固定入口

这个仓库只有一个用途：给员工一个**永远不变的网址**，打开后自动跳转到工作台当前的真实地址。

- `index.html` — 跳转页面（请勿修改）
- `url.txt` — 当前工作台真实网址（**唯一需要更新的文件**）

## 员工指引

收藏这个网址即可，以后工作台网址再变也不用换链接：

> https://ro2sea.github.io/workstation-link/

打开后 1-3 秒自动进入工作台登录页。如果提示「暂时打不开」：等 2-3 分钟再试（页面会自动重试）；仍然打不开就联系沅要最新直连链接。

## 给滢的紧急补救步骤（用 Claude Code，小白友好）

当沅不在、员工说打不开时：

1. 打开你电脑上的 **VSCode**，打开 Claude Code 对话框
2. 把这句话发进去（把【新网址】换成沅微信发你的网址）：

   > 帮我修复工作台固定入口：把 workstation-link 仓库里的 url.txt 内容改成【新网址】，然后 git 提交并推送到 GitHub。

3. 等 Claude 完成即可。员工页面每 30 秒自动重试，最迟约 10 分钟自动恢复，无需通知员工。

**首次使用前**（只需一次）：先让 Claude 做一次准备，把这句话发进去：

> 请 clone https://github.com/Ro2sea/workstation-link 仓库到我的 D 盘「AA-vibe coding」目录下，并配置好 git 推送环境。

如果 Claude Code 用不了，**备用网页版**：打开 https://github.com/Ro2sea/workstation-link/blob/main/url.txt（用你的 GitHub 账号登录）→ 右上角铅笔图标 → 粘贴新网址 → 点两次 Commit changes。

## 维护说明

正常情况下 `url.txt` 由沅电脑上的哨兵程序自动维护（cpolar 网址变化时自动检测并推送更新），**无需任何人手动操作**。手动修改仅用于紧急补救。
