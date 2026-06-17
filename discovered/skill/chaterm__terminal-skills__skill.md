---
name: chaterm__terminal-skills__skill
source: https://github.com/chaterm/terminal-skills/blob/464c2954287ad0c0b9addb1ebfbb2150ddc0de24/devops/ansible/SKILL.md
repo: chaterm/terminal-skills
kind: skill
stars: 45
last_pushed: 2026-03-03T03:28:35Z
license: apache-2.0
score: 8
domains: [devops, automation, infrastructure-as-code]
tags: [ansible, it-operations, iac]
curated: 2026-06-16
curated_by: config-scout
---

# chaterm/terminal-skills — skill

**Why it's worth keeping:** Includes practical, high-value patterns for real-world tasks like rolling updates, dynamic inventory, and vault encryption which are essential for reliable automation.

**Summary:** A comprehensive technical reference covering Ansible workflows from basic ad-hoc commands to advanced role structures and secret management.

**Source credibility:** Solid niche repository focusing on terminal and Kubernetes skills with active maintenance.

**Recency:** Current; updated within the last 4 months.

**Source:** [chaterm/terminal-skills/devops/ansible/SKILL.md](https://github.com/chaterm/terminal-skills/blob/464c2954287ad0c0b9addb1ebfbb2150ddc0de24/devops/ansible/SKILL.md) · 45★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ansible
description: Ansible 自动化运维
version: 1.0.0
author: terminal-skills
tags: [devops, ansible, automation, configuration]
---

# Ansible 自动化运维

## 概述
Playbook 编写、角色管理、动态 inventory 等技能。

## 基础命令

### Ad-hoc 命令
```bash
# 测试连通性
ansible all -m ping
ansible webservers -m ping

# 执行命令
ansible all -m command -a "uptime"
ansible all -m shell -a "df -h | grep /dev"

# 复制文件
ansible all -m copy -a "src=/local/file dest=/remote/file"

# 安装软件
ansible all -m apt -a "name=nginx state=present" --become
ansible all -m yum -a "name=nginx state=present" --become

# 管理服务
ansible all -m service -a "name=nginx state=started" --become

# 收集信息
ansible all -m setup
ansible all -m setup -a "filter=ansible_distribution*"
```

### 常用参数
```bash
-i inventory          # 指定 inventory
-m module             # 指定模块
-a arguments          # 模块参数
-b, --become          # 提权
-K                    # 询问 sudo 密码
-u user               # 指定用户
-k                    # 询问 SSH 密码
--limit host          # 限制主机
-v, -vv, -vvv         # 详细输出
--check               # 检查模式（不执行）
--diff                # 显示差异
```

## Inventory

### 静态 inventory
```ini
# inventory/hosts
[webservers]
web1.example.com
web2.example.com ansible_host
```

</details>
