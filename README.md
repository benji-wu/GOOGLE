# task2_ai_automation.py
# 📌 任務：自動將提示送到 Gemini API 並獲得回應
# ✅ 符合 Task 2 of 4：AI Power-Up 的要求

import os
import google.generativeai as genai

# 設定 API 金鑰（請將 'YOUR_API_KEY' 換成你的金鑰）
GOOGLE_API_KEY = os.getenv("GOOGLE_API_KEY") or "YOUR_API_KEY"
genai.configure(api_key=GOOGLE_API_KEY)

# 初始化 Gemini 模型（使用對話模型）
model = genai.GenerativeModel("gemini-pro")

# 定義提示
prompt = "請用簡單的例子解釋什麼是機器學習？"

# 發送提示並取得回應
response = model.generate_content(prompt)

# 顯示回應
print("🧠 AI 回應：")
print(response.text)

# 將回應儲存到文字檔
with open("ai_response_output.txt", "w", encoding="utf-8") as f:
    f.write(response.text)
    print("\n✅ AI 回應已儲存至 ai_response_output.txt")
