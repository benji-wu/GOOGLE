{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Task 2：提示設計與 AI 測試成果\n",
    "\n",
    "## 🧰 工具選擇與理由\n",
    "\n",
    "本任務使用以下工具進行提示工程探索：\n",
    "\n",
    "- **Google Colab**：提供雲端運算資源，便於執行 Python 程式與測試提示，無需本機安裝環境。\n",
    "- **Google Gemini API**：支援自然語言處理與多模態輸入，能快速產生 AI 回應，適合用於提示測試與調整。\n",
    "\n",
    "這些工具整合性高、使用門檻低，特別適合用於教育場域與互動實驗。"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Prompt 1：資訊查詢型 - 解釋量子電腦\n",
    "\n",
    "**Prompt：**\n",
    "請用簡單的語言向國中生解釋什麼是量子電腦。\n",
    "\n",
    "**AI 回應：**\n",
    "量子電腦不像一般電腦只用 0 和 1，它能同時表示多種狀態。\n",
    "就像你在玩彈珠機時，一顆球可以同時在兩個軌道上搖擺，直到你觀察它。\n",
    "這讓它在某些計算上比普通電腦更快、更有效率。"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Prompt 2：創意寫作型 - 孤獨的機器人詩\n",
    "\n",
    "**Prompt：**\n",
    "請創作一首短詩，主題為「孤獨的機器人」。\n",
    "\n",
    "**AI 回應：**\n",
    "他站在夜色下  \n",
    "孤單閃著紅燈  \n",
    "心跳像沒電般  \n",
    "尋找誰能聽懂"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Prompt 3：程式生成型 - 判斷質數\n",
    "\n",
    "**Prompt：**\n",
    "請使用 Python 寫一段程式碼，判斷使用者輸入的數字是否為質數。\n",
    "\n",
    "**AI 回應：**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "# 判斷是否為質數\n",
    "num = int(input(\"請輸入一個數字：\"))\n",
    "if num > 1:\n",
    "    for i in range(2, num):\n",
    "        if num % i == 0:\n",
    "            print(\"不是質數\")\n",
    "            break\n",
    "    else:\n",
    "        print(\"是質數\")\n",
    "else:\n",
    "    print(\"不是質數\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Prompt 4：邏輯推理型 - 誰最高？\n",
    "\n",
    "**Prompt：**\n",
    "小明比小華高，小華比小美矮。誰最高？請用 50 字內解釋給小學生聽。\n",
    "\n",
    "**AI 回應：**\n",
    "小明最高，因為他比小華高，小華又比小美高，所以小明比大家都高。"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Prompt 5：風格轉換型 - 莎士比亞語氣\n",
    "\n",
    "**Prompt：**\n",
    "請將「我今天心情不好」翻譯為莎士比亞語氣。\n",
    "\n",
    "**AI 回應：**\n",
    "一般翻譯：I am in a bad mood today.  \n",
    "莎士比亞風格：Verily, mine heart doth weep this day."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Prompt 6：分類任務型 - 判斷情緒語氣\n",
    "\n",
    "**Prompt：**\n",
    "請判斷句子情緒：「這部電影劇情拖沓，但演員表現不錯。」\n",
    "\n",
    "**AI 回應：**\n",
    "情緒傾向：中性偏負面。  \n",
    "理由：雖有演員表現佳的正面元素，但整體語氣以批評劇情為主。"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "name": "python",
   "version": "3.9"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
