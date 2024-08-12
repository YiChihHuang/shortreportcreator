# 研究報告生成工具

此專案是一個基於Python的工具，旨在自動化生成繁體中文研究報告的過程。該工具結合了OpenAI的GPT-4模型和Tavily API，從指定來源搜尋相關信息並生成報告。生成的報告將以Word文檔格式保存，方便後續下載和使用。

本專案受到了[assafelovic/gpt-researcher](https://github.com/assafelovic/gpt-researcher)專案的啟發，特此致謝。

Colab:[shortreportcreater 0812](https://colab.research.google.com/drive/15YJIVi_7i18X25GlkEvxqOU1EEBM_au1?usp=sharing)

## 功能特點

- **自動搜尋**：使用Tavily API在指定來源或所有可用來源中搜尋相關信息。
- **報告生成**：利用OpenAI API生成結構化的繁體中文研究報告，包含引言、主要研究發現、討論和結論。
- **Word文檔生成**：將生成的報告格式化並保存為`.docx`文件，隨後可自動下載。

## 環境需求

- Python 3.x
- 必要的Python套件（可通過`pip`安裝）：
  - `openai`
  - `tavily`
  - `python-docx`
  - `python-dotenv`

## 安裝步驟

- 1. 複製此儲存庫：
   ```bash
   git clone https://github.com/your-username/research-report-generator.git
   cd research-report-generator

- 2. 安裝所需的Python套件## 
  ```bash
  pip install -r requirements.txt

- 3. 設置環境變量。您可以在專案根目錄中創建一個 .env 文件，內容如下：
  ```env
  OPENAI_API_KEY=your_openai_api_key_here
  TAVILY_API_KEY=your_tavily_api_key_here

- 4. 運行腳本
  ```bash
  python generate_report.py

## 使用說明
  - 1. 當系統提示時，輸入您想生成報告的研究主題。
  - 2. 提供資訊來源，您可以選擇：
    -  輸入 all 搜索所有可用來源。
    -  或者指定最多5個URL（用逗號分隔），僅從這些來源中搜索信息。
  - 3. 工具將搜尋信息，生成報告並保存為Word文檔。
  - 4. 生成的Word文檔將自動下載至您的本地電腦。



