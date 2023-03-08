# dayOfyear
a simple code
"""
----------定义全局变量------------
"""
money = 5000000
name = None
"""
-----------定义函数----------
"""
# 定义查询余额函数
def querying():
    print("---------查询余额----------")
    print(f"周杰伦，您好，你的余额剩余：{money}元")
# 定义存款函数
def save():
    print("----------存款------------")
    save_num = int(input("您要存多少钱："))
    global money
    money += save_num
    print(f"周杰伦，您好，您存款{save_num}元成功")
    print(f"周杰伦，您好，你的余额剩余：{money}元")
# 定义取款函数
def take():
    print("----------取款------------")
    take_num = int(input("您要取多少钱："))
    global money
    money -= take_num
    print(f"周杰伦，您好，您取款{take_num}元成功")
    print(f"周杰伦，您好，你的余额剩余：{money}元")
# 定义主菜单函数
def menu():
    print("----------主菜单----------")
    print("周杰伦，您好，欢迎来到黑马银行ATM。请选择操作：")
    print("查询余额\t【输入1】")
    print("存款\t\t【输入2】")
    print("取款\t\t【输入3】")
    print("退出\t\t【输入4】")
    num1 = int(input("请输入您的选择："))
    return num1

"""
-------------主函数------------
"""
name = input("请输入您的名字：")
if name == "周杰伦":
    while True:
        keyboard_input = menu()
        if keyboard_input == 1:
            querying()
        elif keyboard_input == 2:
            save()
        elif keyboard_input == 3:
            take()
        else:
            print("程序退出了！")
            break
else:
    print("你输入的名字错误")
