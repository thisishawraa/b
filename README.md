def linear_search(arr, target):
    for index, element in enumerate(arr):  # نمر على كل عنصر مع موقعه في القائمة
        if element == target:  # إذا كان العنصر يساوي القيمة المطلوبة
            return index  # نرجع موقع العنصر
    return -1  # إذا لم يتم العثور على العنصر

# مثال
array = [5, 3, 8, 4, 2]

while True:
    target = int(input("أدخل القيمة المراد البحث عنها: "))
    result = linear_search(array, target)

    if result != -1:
        print(f"العنصر {target} موجود في الموقع {result}.")
    else:
        print(f"العنصر {target} غير موجود في القائمة.")
