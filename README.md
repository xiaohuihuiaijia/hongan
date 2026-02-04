# 红岸团队代码库

欢迎来到红岸团队的代码仓库！本仓库用于统一管理团队的研发项目代码和项目数据。

## 目录结构

```
hongan/
├── projects/           # 各项目代码目录
├── project-data/       # 各项目数据目录（业务数据、样本数据等）
└── shared/             # 共享组件、工具库
```

### 目录说明

| 目录 | 用途 |
|------|------|
| `projects/` | 存放所有项目的代码，每个项目一个子目录 |
| `project-data/` | 存放各项目的业务数据和样本数据 |
| `shared/` | 存放团队共享的工具、组件、脚本等 |

## 快速开始

### 克隆仓库

```bash
git clone git@github.com:YOUR_USERNAME/hongan.git
cd hongan
```

### 创建新项目

```bash
# 创建项目代码目录
mkdir projects/my-project

# 创建对应的数据目录
mkdir project-data/my-project
```

## Git 常用命令

### 基础操作

| 命令 | 说明 | 示例 |
|------|------|------|
| `git clone <url>` | 克隆远程仓库 | `git clone git@github.com:user/repo.git` |
| `git add <file>` | 添加文件到暂存区 | `git add .` 或 `git add README.md` |
| `git commit -m "msg"` | 提交更改 | `git commit -m "feat: 添加新功能"` |
| `git push` | 推送到远程仓库 | `git push origin main` |
| `git pull` | 拉取远程更新 | `git pull origin main` |

### 分支管理

| 命令 | 说明 | 示例 |
|------|------|------|
| `git branch` | 查看本地分支 | `git branch` |
| `git branch <name>` | 创建新分支 | `git branch feature/login` |
| `git checkout <branch>` | 切换分支 | `git checkout develop` |
| `git checkout -b <name>` | 创建并切换分支 | `git checkout -b feature/login` |
| `git merge <branch>` | 合并分支 | `git merge feature/login` |
| `git branch -d <name>` | 删除已合并的分支 | `git branch -d feature/login` |

### 状态查看

| 命令 | 说明 | 示例 |
|------|------|------|
| `git status` | 查看工作区状态 | `git status` |
| `git log` | 查看提交历史 | `git log --oneline -10` |
| `git diff` | 查看未暂存的更改 | `git diff` |
| `git diff --staged` | 查看已暂存的更改 | `git diff --staged` |

### 远程操作

| 命令 | 说明 | 示例 |
|------|------|------|
| `git remote -v` | 查看远程仓库 | `git remote -v` |
| `git remote add <name> <url>` | 添加远程仓库 | `git remote add origin <url>` |
| `git fetch` | 获取远程更新（不合并） | `git fetch origin` |

### 撤销操作

| 命令 | 说明 | 示例 |
|------|------|------|
| `git checkout -- <file>` | 撤销工作区修改 | `git checkout -- README.md` |
| `git reset HEAD <file>` | 取消暂存 | `git reset HEAD README.md` |
| `git reset --soft HEAD~1` | 撤销上次提交（保留更改） | `git reset --soft HEAD~1` |
| `git revert <commit>` | 创建新提交来撤销指定提交 | `git revert abc123` |

## 贡献规范

### 分支命名

| 类型 | 格式 | 示例 |
|------|------|------|
| 新功能 | `feature/<描述>` | `feature/user-login` |
| Bug修复 | `bugfix/<描述>` | `bugfix/fix-crash` |
| 热修复 | `hotfix/<描述>` | `hotfix/security-patch` |
| 发布 | `release/<版本>` | `release/v1.0.0` |

### 提交信息格式

建议使用 [Conventional Commits](https://www.conventionalcommits.org/) 规范：

```
<类型>: <描述>

[可选的详细说明]
```

**类型说明：**

| 类型 | 说明 |
|------|------|
| `feat` | 新功能 |
| `fix` | Bug 修复 |
| `docs` | 文档更新 |
| `style` | 代码格式（不影响功能） |
| `refactor` | 代码重构 |
| `test` | 测试相关 |
| `chore` | 构建/工具相关 |

**示例：**

```bash
git commit -m "feat: 添加用户登录功能"
git commit -m "fix: 修复首页加载缓慢问题"
git commit -m "docs: 更新 README 文档"
```

## 团队成员

红岸团队 - 持续创新，追求卓越

---

如有问题，请联系团队管理员。
