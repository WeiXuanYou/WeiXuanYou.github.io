---
title: "Vivado Synthesis Timing Violation... Again"
date: 2025-12-10
tags: ["FPGA", "Vivado", "Debug"]
summary: "Negative Slack -0.4ns. The joy of hardware design."
---

花了整整兩天把 YOLO 的後處理 (Post-processing) 寫進 PL 端。
結果 Synthesis 一跑完：**Worst Negative Slack (WNS): -0.45ns**。🔴

看來是 Critical Path 太長，卡在某個乘法器後面。
只好乖乖回去加 Pipeline Register 切割時序了。
軟體工程師真的很幸福，多寫一行 code 只要幾秒鐘；硬體工程師多加一個 stage，要重跑 30 分鐘 Synthesis... ☕
