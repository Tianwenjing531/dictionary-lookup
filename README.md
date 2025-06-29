# dictionary-lookup
 我的第一个 Python 项目：英汉字典查询小程序（可选）
# 定义一个英汉字典
dictionary = {
    "apple": "苹果",
    "banana": "香蕉",
    "book": "书",
    "computer": "电脑",
    "python": "蟒蛇 / 编程语言"
}

print("欢迎使用英汉字典查询器（输入 q 退出）")

while True:
    word = input("请输入要查询的单词：").lower()  # 用户输入，转为小写
    if word == "q":
        print("感谢使用，再见！")
        break
    elif word in dictionary:
        print(f"{word} 的中文意思是：{dictionary[word]}")
    else:
        print("对不起，词库中没有这个单词。")
