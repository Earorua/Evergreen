# Evergreen

[简体中文](README.md) | **English**

**Elder Care Foundation Management Platform**

A management platform for elder care foundations, bringing together donations, personnel, gifts, events, and finance with visual analytics and intelligent data queries to support daily operations and management decisions.

## Features

- Donation management: Donation records, donors, categories, feedback, and tax receipts.
- Personnel management: Employee and volunteer records, schedules, a schedule board, and compensation.
- Gifts and events: Gift inventory, batches, distribution, delivery, suppliers, and event planning.
- Financial management: Grants, other income, and financial reports.
- Data analytics: Dashboards, self-service BI, and natural-language read-only queries with result explanations through OpenRouter.
- Administration and collaboration: Role-based access control, English/Chinese interfaces, and system improvement suggestions.

## Run Locally

Tech stack: Flask, Jinja2, Bootstrap 5, Flask-Login, and SQLite.

```bash
git clone https://github.com/Earorua/Evergreen.git
cd Evergreen
pip install -r requirements.txt
python app.py
```

Open [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser. The project includes a sample database. See the [user manual (Chinese)](USER_MANUAL.md) for demo accounts and detailed instructions.

To use intelligent data queries, set the `OPENROUTER_API_KEY` environment variable before starting the app. See the user manual for configuration details. Do not commit API keys to the repository.

## Verification

```bash
python -m unittest discover
```

## Project Background

This project was developed as coursework with assistance from Claude Code and Codex.

[Course Project Outline](https://github.com/user-attachments/files/26561894/Project_Outline.pdf)
