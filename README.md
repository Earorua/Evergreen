# Evergreen

**简体中文** | [English](README.en.md)

**养老公益基金会管理平台**

面向养老公益基金会的综合管理平台，整合捐赠、人员、物资、活动与财务管理，并提供可视化分析和智能数据查询，支持机构的日常运营与管理决策。

## 主要功能

- 捐赠管理：捐赠记录、捐赠者、分类、反馈与税务收据。
- 人员管理：员工与志愿者信息、排班、排班看板与薪酬。
- 物资与活动：礼品库存、批次、分发、配送、供应商与活动策划。
- 财务管理：拨款、其他收入与财务报表。
- 数据分析：仪表盘、BI 自助分析，以及通过 OpenRouter 提供的自然语言只读查询与结果解读。
- 协作管理：角色权限、中英文切换与系统优化建议。

## 本地运行

技术栈：Flask、Jinja2、Bootstrap 5、Flask-Login、SQLite。

```bash
git clone https://github.com/Earorua/Evergreen.git
cd Evergreen
pip install -r requirements.txt
python app.py
```

在浏览器打开 [http://127.0.0.1:5000](http://127.0.0.1:5000)。项目内置示例数据库，预置账户及完整操作说明见 [用户手册](USER_MANUAL.md)。

智能数据查询需要在启动前设置环境变量 `OPENROUTER_API_KEY`，具体配置见用户手册。API 密钥不应提交到仓库。

## 验证

```bash
python -m unittest discover
```

## 项目背景

本项目为课程实践，借助 Claude Code 与 Codex 完成。

[课程项目说明（Project Outline）](https://github.com/user-attachments/files/26561894/Project_Outline.pdf)
