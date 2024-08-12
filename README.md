#研究報告生成工具


此專案是一個基於Python的工具，旨在自動化生成繁體中文研究報告的過程。該工具結合了OpenAI的GPT-4模型和Tavily API，從指定來源搜尋相關信息並生成報告。生成的報告將以Word文檔格式保存，方便後續下載和使用。

本專案受到了assafelovic/gpt-researcher專案的啟發，特此致謝。

#功能特點
自動搜尋：使用Tavily API在指定來源或所有可用來源中搜尋相關信息。
報告生成：利用OpenAI API生成結構化的繁體中文研究報告，包含引言、主要研究發現、討論和結論。
Word文檔生成：將生成的報告格式化並保存為.docx文件，隨後可自動下載。

#環境需求
Python 3.x
必要的Python套件（可通過pip安裝）：
openai
tavily
python-docx
python-dotenv

#安裝步驟
複製此儲存庫：


bash
複製程式碼
git clone https://github.com/your-username/research-report-generator.git
cd research-report-generator
安裝所需的Python套件：


bash
複製程式碼
pip install -r requirements.txt
設置環境變量。您可以在專案根目錄中創建一個 .env 文件，內容如下：

env
複製程式碼
OPENAI_API_KEY=your_openai_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here
運行腳本：

bash
複製程式碼
python generate_report.py


#使用說明
當系統提示時，輸入您想生成報告的研究主題。
提供資訊來源，您可以選擇：
輸入 all 搜索所有可用來源。
或者指定最多5個URL（用逗號分隔），僅從這些來源中搜索信息。
工具將搜尋信息，生成報告並保存為Word文檔。
生成的Word文檔將自動下載至您的本地電腦。
使用範例
以下是工具使用的快速範例：

bash
複製程式碼
請輸入研究主題: 生成式AI手機的定義與特徵
請輸入資訊來源 (輸入 'all' 搜索所有來源，或輸入至多5個指定url，用逗號分隔): all
系統將輸出：

makefile
複製程式碼
研究報告已生成並保存至 生成式AI手機的定義與特徵_研究報告.docx
報告內容預覽:
(500個字符的報告預覽)...
貢獻指南
如果您有任何建議或改進，歡迎提交問題或拉取請求。

授權條款
此專案基於MIT許可證進行授權 - 有關詳細信息，請參閱LICENSE文件。

