# 📊 半导体测试数据转换工具 (Semiconductor Test Data Converter)

这是一个基于 **Streamlit** 开发的轻量级 Web 工具，专门用于将半导体测试生成的 CSV 数据文件转换为标准化的 TXT 或 MEA 格式。

---

## ✨ 主要功能

* **自动化参数解析**：能够根据文件名自动提取关键参数（如 $L$ 值和 $V_{ds}$）。
* **批量转换**：支持一次性上传多个 CSV 文件并进行批量处理。
* **灵活配置**：
    * 支持手动覆盖 $L$、W 和 $V_{ds}$ 参数。
    * 支持反转 `Curve`（Vbs）的替换顺序，应对数据采集方向不同的情况。
* **多格式输出**：转换结果支持 `.txt` 和 `.mea` 两种后缀。
* **一键打包**：处理多个文件时，支持以 ZIP 压缩包形式一键下载。

---

## 🚀 快速上手

### 1. 准备环境
确保你的电脑已安装 Python 3.8+，然后安装依赖：
```bash
pip install -r requirements.txt

# 启动 Web UI
streamlit run app.py
