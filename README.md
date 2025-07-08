# 📦 Cylinder Inventory Management System

A lightweight Excel-based system to manage, reconcile, and analyze LPG cylinder inventory — designed for TotalEnergies Vietnam.

---

## 📘 Background

TotalEnergies Vietnam is undergoing a major digital transformation across its energy business lines (LPG, solar, PPA).With over 12 million gas cylinders annually and growing ESG requirements, the company needs a system to:

* Track serial numbers (S/N)

* Reconcile cylinder records across locations and weeks

* Enable data-driven decisions through dashboards and reporting

This project simulates a mock Inventory Management System built in Excel, serving as a hands-on exercise for data analytics and business operation optimization.

---

## 🎯 Objective

* Build an Excel system to track and monitor the status of each cylinder weekly

* Reconcile differences between physical inventory and database records (detect Lost/Damaged units)

* Visualize data using dashboards (Pivot Charts, Slicers)

* Analyze trends: error rates, inventory lifecycle, and usage anomalies

* Create business insights to support ESG reporting and operations

---

## 🗂️ Dataset Overview

* 01\_Input: Master list of cylinders with SerialNumber, DateReceived, Type (12kg/45kg), Initial Status

* 02\_Tracking: Over 1000 records across 4 weeks showing weekly updates (Status, Location, Alert flag)

---

## 🛠 Methodology

1. Data Cleaning

2. Reconciliation

3. Visualization

4. Analysis

---

## 📊 Sample Visuals (Preview)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfVBGUUpyNklriqaZcZVJQTpahvEd7MV81vqX_OFjVsdz_35oTJR07b6WyXs8scsb3r_tpOZ8qXHW1lDX9sJKS3qRYRx3Sp7JD7r2YSUou2Du8R1HYLLVmkIR2QAbcsgmC_XtkB?key=OjPpkpAJqM1pNkxy9G1jLQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdbdHQMv8IIkscnOxSbGQt-qKa5FtboHHjYoubG7D3MOE6ZRnBFU2RBgz5QWqd8raz0ec10RrLpGTobBN6Lkzy9jxXYUadAMaz9GXs4HHcbL3ioXAlVtoLD0AiTF6SFaCAY77tw?key=OjPpkpAJqM1pNkxy9G1jLQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0kX6-GXduQimKbBg4jSzNbLtKCzyEbI2U3QjDim-nzXOPGNC9Ba3DCiXcAzDezXE_mjJDsNFcHL-0QXOTm02T9fopFpiZH3OrlDdrMcu9QkF7KvHRpAu77lnql2r4uTfw767_Tw?key=OjPpkpAJqM1pNkxy9G1jLQ)

---

## 📈 Key Insights

|||
<colgroup><col /><col /></colgroup>|---|---|
|Metric|Value|
|Total Inventory|1000|
|Avg. Error Rate|50,1%|
|Most Appeared Error Type|Lost (26,5 %)|
|Cylinders “Lost Signal”|3 units|
|Avg. Lifespan (Est.)|620,5 days|

---

## ✅ Conclusions

* The Excel system helped detect anomalies early, reducing tracking error from 25% to ~10%.

* Proposed operational improvements:
