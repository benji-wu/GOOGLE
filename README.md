import openai

# 🔐 你的 OpenAI API 金鑰
openai.api_key = "YOUR_API_KEY"  # <- 替換成你的 API 金鑰

def explain_topic(topic: str):
    prompt = f"""
你是一位國中自然老師，請用 3 段話循序漸進地解釋「{topic}」，每段不超過 50 字，並舉生活例子幫助學生理解。
"""
    response = openai.ChatCompletion.create(
        model="gpt-3.5-turbo",
        messages=[
            {"role": "user", "content": prompt}
        ],
        temperature=0.7
    )

    explanation = response.choices[0].message.content.strip()
    return explanation

# ✅ 範例輸出
topic = "量子電腦"
print("🔍 主題：", topic)
print(explain_topic(topic))
