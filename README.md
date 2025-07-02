# 質數檢查程式
num = int(input("請輸入一個正整數："))

# 質數定義：除了 1 和自己之外，不能被其他整除
if num > 1:
    for i in range(2, num):
        if num % i == 0:
            print(num, "不是質數")
            break
    else:
        print(num, "是質數")
else:
    print(num, "不是質數")

# 範例：
# 輸入：7 ➜ 是質數
# 輸入：9 ➜ 不是質數
