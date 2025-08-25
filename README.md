# Homework4

# 🧱 HR 管理系統 - MVC 架構專案

本專案採用 Java Swing + DAO + Service + MVC 架構，實作員工出勤與請假管理功能。


## 📦 專案架構
```
Model/
├── AttendanceLog.java
├── Employee.java
├── LeaveLog.java
DAO/
├── AttendanceLogDao.java
    ├── AttendanceLogDaoImpl.java
├── EmployeeDao.java
    ├── EmployeeDaoImpl.java
├── LeaveLogDao.java
    ├── LeaveLogDaoImpl.java
Service/
├── AttendanceLogService.java
    ├── AttendanceLogServiceImpl.java
├── EmployeeService.java
    ├── EmployeeServiceImpl.java
├── LeaveLogService.java
    ├── LeaveLogServiceImpl.java
Util/
├── CheckCode.java
├── DbConnection.java
├── Tool.java
Controller/
├── HomePageUnlogin.java
    ├── LoginPage.java
        ├── HomePage.java
        ├── AttendanceLogPage.java
        ├── LeaveLogPage.java
        ├── InformationPage.java
        └── HRPage.java
```


## 🧭 架構說明

- **Model 層**：封裝資料結構，對應資料庫表格。
- **DAO 層**：資料存取邏輯，負責 SQL 操作。
- **Service 層**：業務邏輯處理，串接 DAO 與 Controller。
- **Util 工具層**：提供驗證碼、資料庫連線、報表文案內容等共用工具。
- **Controller 層**：Swing UI 介面，處理使用者互動。

## 🚀 執行方式

1. 使用 IDE 開啟專案（如 IntelliJ 或 Eclipse）
2. 設定資料庫連線（參考 `DbConnection.java`）
3. 執行 `LoginPage.java` 進入系統

## 📌 功能特色

- 員工登入與驗證
- 出勤紀錄查詢與新增
- 請假申請與審核
- Swing UI 模組化設計
- DAO/Service 分層架構，易於維護

## 📚 技術棧

- Java SE
- Swing UI
- JDBC + MySQL
- MVC 架構
- Markdown 語法


