---
title: "Featured Projects"
---

### 🛠️ EDA & Optimization
#### **Intelligent Power/Ground Routing System** (Current Work)
* **Challenge**: 傳統 EDA 工具在處理極端製程下的電源網路合成時，常面臨繞線擁塞與 IR Drop 問題。
* **Solution**: 開發基於 Python/C++ 的自動化路由引擎，並實驗性引入 **Reinforcement Learning** 進行路徑規劃決策。
* **Tech**: C++, Python, Graph Theory, Voronoi/Delaunay.

### 🤖 AI & LLM
#### **Gemma-Based Voice Assistant (Personal Project)**
* **Goal**: 打造一個離線、高隱私的家庭語音助理。
* **Architecture**: 
    * **Edge**: Raspberry Pi 負責語音採集 (VAD) 與喚醒詞偵測。
    * **Server**: Desktop (RTX 4070 Ti) 運行 Fine-tuned Gemma-7B/270M 模型處理指令。
    * **Backend**: Django 處理業務邏輯與設備控制。
* **Status**: *In Development (Training Phase)*

### ⚡ Hardware & FPGA
#### **FPGA Object Detection Accelerator** (Master's Thesis)
* **Overview**: 針對邊緣裝置資源受限問題，設計軟硬體協同加速器。
* **Key Result**: 使用 Vitis HLS 優化卷積運算單元，成功在 PYNQ-Z2 上實現即時物件偵測。
* **Tech**: Xilinx Vitis AI, PYNQ, C++, PyTorch.