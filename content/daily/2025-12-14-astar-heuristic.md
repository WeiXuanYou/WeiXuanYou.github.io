---
title: "[DevLog] Tuning A* Heuristic for Power Routing"
date: 2025-12-14
tags: ["EDA", "Algorithm", "C++"]
summary: "Admissible heuristic is safe, but too slow. Trying to over-estimate today."
---

今天在調整 Global Router 的 A* 演算法。
原本堅持用 Admissible Heuristic (保證最短路徑)，但在 3nm 複雜度下搜尋空間實在太大，Run time 直接爆炸 💥。

下午嘗試把 H-cost 權重拉高 (Over-estimation)，雖然犧牲了一點點線長最佳解，但收斂速度快了 **40%**。
這就是工程上的 Trade-off 吧。明天再來跑個 DRV (Design Rule Check) 看看有沒有違規。
