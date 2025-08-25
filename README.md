# Homework4

# 🧱 HR 管理系統 - MVC 架構專案

本專案以 Java Swing MVC 架構實作，並將資料處理流程細分為 DAO 層（資料存取）、Service 層（商業邏輯）與 Controller 層（介面控制），完成員工出勤與請假管理功能。


## 📦 專案架構
```
Model/
├── AttendanceLog.java
├── Employee.java
├── LeaveLog.java
DAO/
├── AttendanceLogDao.java
    └── AttendanceLogDaoImpl.java
├── EmployeeDao.java
    └── EmployeeDaoImpl.java
├── LeaveLogDao.java
    └── LeaveLogDaoImpl.java
Service/
├── AttendanceLogService.java
    └── AttendanceLogServiceImpl.java
├── EmployeeService.java
    └── EmployeeServiceImpl.java
├── LeaveLogService.java
    └── LeaveLogServiceImpl.java
Util/
├── CheckCode.java
├── DbConnection.java
├── Tool.java
Controller/
└── HomePageUnlogin.java
    └── LoginPage.java
        ├── HomePage.java
        ├── AttendanceLogPage.java
        ├── LeaveLogPage.java
        ├── InformationPage.java
        └── HRPage.java
```


## 🧭 架構說明

◎ Model：資料結構與資料庫對應。

◎ DAO：資料存取層，執行 SQL 操作。

◎ Service：業務邏輯層，整合 DAO 與 Controller。

◎ Util：共用工具，例如驗證碼、資料庫連線與報表。

◎ Controller：UI 控制層，處理使用者互動與流程。

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

