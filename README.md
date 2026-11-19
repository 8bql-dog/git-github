# git与github绑定

用于练习和记录 Git 本地仓库与 GitHub 远程仓库的绑定流程。

## 环境

- Git 2.56.1（安装路径 `D:\Git`）
- 默认分支：`main`

## 常用流程

```bash
# 1. 初始化本地仓库
git init -b main

# 2. 配置提交身份
git config user.name "你的名字"
git config user.email "你的邮箱"

# 3. 首次提交
git add .
git commit -m "Initial commit"

# 4. 关联远程仓库并推送
git remote add origin <仓库地址>
git push -u origin main
```

## 认证方式

- HTTPS：使用 GitHub 个人访问令牌（PAT）替代密码，可用凭据管理器缓存
- SSH：本地生成密钥对，将公钥添加到 GitHub 账号

## 记录

- 2026-11-19：初始化本地仓库，建立首个提交
