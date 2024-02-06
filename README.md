
ls = []
while 1 > 0:
    b = int(input("yozish 1\no'chirish 2\nchiqish 0\nSon kiriting: "))
    if b == 1:
        n = int(input("boshiga 1\noxiriga 2\nindexga 3\nKiriting: "))
        if n == 1:
            q = int(input("nechta malumot qoshmmoqchisiz: "))
            print("nima qo'shmoqchisiz: ")
            for i in range(q):
                ls.insert(0, input())
        elif n == 2:
            q = int(input("oxiriga nechta malumot qoshmmoqchisiz: "))
            print("nima qo'shmoqchisiz: ")
            for i in range(q):
                ls.append(input())
        elif n == 3:
            z = int(input("Nechanchi indexga qoshmoqchsiz: "))
            print(z, " - indexga nima qoshmoqchisiz", ls.insert(z,input("kiriting: ")))
        print("LIST:  ", ls)
        print("\n\n\n")
    elif b == 2:
        if ls == []:
            print("list bosh ochirgani hech narsa yoq")
            continue
        m = int(input("listni oxiridan o'chirish 1\nlistni indexdan o'chirish 2\nlistni qiymatni o'chirish 3\nlistni to'zalab beradi 4\nSon kiriting: "))
        if m == 1:
            ls.pop()
        elif m == 2:
            g = int(input("nechanchi indexni ochirmoqchisiz: "))
            ls.pop(g)
        elif m == 3:
            print(ls)
            r = input("nimani ochirmoqchisiz: ")
            ls.remove(r)
        elif m == 4:
            ls.clear()

        if b == 0:
            os.system("cls")
            break
        print("LIST:  ",ls)
        print("\n\n\n")
