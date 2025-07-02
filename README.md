# 使用者輸入數字
num = int(input("請輸入一個整數："))

# 檢查是否為質數
if num > 1:
    for i in range(2, num):
        if num % i == 0:
            print(num, "不是質數")
            break
    else:
        print(num, "是質數")
else:
    print(num, "不是質數")

# 範例輸入：7
# 範例輸出：7 是質數
