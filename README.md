# CRMS 電腦維修系統

這是一個基於 Flask 的電腦維修管理系統（Computer Repair Management System），提供使用者報修、管理員派工、工程師維修狀態更新，以及簡易 AI 查詢功能。

## 功能特色

- 使用者登入與角色權限
- 建立報修單
- 管理員派工給工程師
- 工程師更新維修狀態
- 基礎儀表板頁面
- AI 查詢：可查詢待處理案件、我的報修單、已完成案件與案件統計

## 技術堆疊

- Python 3.10+
- Flask
- Flask-SQLAlchemy
- SQLite
- Jinja2 Templates
- pytest

## 安裝方式

1. 進入專案目錄

```bash
cd computer_repair_system
```

2. 建立虛擬環境

```bash
python -m venv .venv
```

3. 啟動虛擬環境

Windows PowerShell：

```powershell
.\.venv\Scripts\Activate.ps1
```

4. 安裝依賴

```bash
pip install -r requirements.txt
```

## 啟動應用

```bash
python app.py
```

啟動後可透過瀏覽器開啟：

```text
http://127.0.0.1:5000
```

## 預設帳號

- 管理員
  - 帳號：admin
  - 密碼：1234

- 工程師
  - 帳號：eng
  - 密碼：1234

- 一般使用者
  - 帳號：user
  - 密碼：1234

## AI 查詢使用方式

登入後進入使用者儀表板，可在 AI 查詢欄位輸入以下類型問題：

- 列出待處理的案件
- 我的報修單
- 已完成案件
- 案件統計

## 測試

```bash
python -m pytest -q
```
