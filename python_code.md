# dayOfyear
a simple code
import random
num = random.randint(1, 10)
print(num)
temp = int(input("1.请输入您猜测的数字："))
if temp == num:
    print("恭喜你，第一次就猜对了。")
else:
    if temp > num:
        print("猜大了。")
    else:
        print("猜小了")
    temp = int(input("2.请输入您猜测的数字："))
    if temp == num:
        print("恭喜你，第二次猜对了。")
    else:
        if temp > num:
            print("猜大了。")
        else:
            print("猜小了.")
        temp = int(input("3.请输入您猜测的数字："))
        if temp == num:
            print("恭喜你，最后一次就猜对了。")
        else:
            print("机会用完了，没有猜对。")
