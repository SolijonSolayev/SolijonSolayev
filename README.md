def kalkulyator():
    print("Soddalashtirilgan kalkulyator")
    while True:
        try:
            num1 = float(input("Birinchi sonni kiriting: "))
            operator = input("Amalni tanlang (+, -, *, /): ")
            num2 = float(input("Ikkinchi sonni kiriting: "))

            if operator == "+":
                natija = num1 + num2
            elif operator == "-":
                natija = num1 - num2
            elif operator == "*":
                natija = num1 * num2
            elif operator == "/":
                natija = num1 / num2
            else:
                print("Noto'g'ri amalni tanladingiz. Qaytadan kiriting.")
                continue

            print("Natija: ", natija)

            davom = input("Yana hisoblashni istaysizmi? (ha/yuq): ")
            if davom.lower() != 'ha':
                break
        except ValueError:
            print("Xatolik! Son kiriting.")
        except ZeroDivisionError:
            print("Xatolik! Nolga bo'lish mumkin emas.")

kalkulyator()


<!---
SolijonSolayev/SolijonSolayev is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
