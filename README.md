# macrodroid-examples

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)]()
[![Made with MacroDroid](https://img.shields.io/badge/Made%20with%20MacroDroid-orange.svg)]()
[![GitHub last commit](https://img.shields.io/github/last-commit/kamonomichi/macrodroid-examples)]()

A collection of **real-world MacroDroid automations** and `.macro` files  
verified on actual Android devices.

This repository is designed for:

- Users who want **reproducible automation workflows**
- Developers exploring **Android OS–aware macro design**
- Learners who prefer **hands-on examples over theory**
- Anyone who wants to understand **Trigger → Action → Constraint** logic patterns

All examples originate from  
https://kamonomichi.com/  
and are optimized for clarity, reproducibility, and practical use.

---

## 🔧 Technical Overview

MacroDroid is a powerful automation tool, but its behavior is heavily influenced by:

- Android OS version  
- Manufacturer restrictions（Xiaomi / OPPO / Samsung / Pixel 等）  
- Permission states  
- Background execution limits  
- Accessibility service stability  
- 通知・センサー・UI操作の OS 仕様差分  

Because of this, each macro in this repository includes **technical context**, not just the `.macro` file.

### Each example documents:

- **Trigger rationale**（なぜそのトリガーを選ぶか）
- **Action logic**（実行内容の因果関係）
- **Constraint design**（誤作動防止の条件）
- **OS / device considerations**（Androidバージョン差分）
- **実機検証メモ**（再現性の担保）

This makes the repository a **knowledge base for Android automation design**,  
not just a macro collection.

---

## 📚 Examples

→ **[View all examples](examples.md)**

Examples include:

- Daily automation  
- UI automation（タップ/スワイプ/通知操作）  
- Context-aware workflows  
- Battery/permission-safe designs  
- OS差分に強い安定化パターン  

---

## 📸 Screenshot

![MacroDroid Example Screenshot](https://raw.githubusercontent.com/kamonomichi/macrodroid-examples/main/share_842429301686638893.jpg)

---

## 🧩 Folder Structure

