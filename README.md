def linear_search(arr, target):
    for index, element in enumerate(arr):  # المرور على كل عنصر في القائمة
        if element == target:  # إذا كان العنصر يساوي القيمة المطلوبة
            return index  # إرجاع موقع العنصر
    return -1  # إرجاع -1 في حال عدم العثور على العنصر

# القائمة
array = [5, 3, 8, 4, 2]

# تنفيذ البرنامج
while True:
    try:
        target = int(input("أدخل القيمة المراد البحث عنها: "))  # طلب إدخال قيمة من المستخدم
        result = linear_search(array, target)  # استدعاء الدالة

        if result != -1:
            print(f"العنصر {target} موجود في الموقع {result}.")
        else:
            print(f"العنصر {target} غير موجود في القائمة.")
    except ValueError:
        print("من فضلك أدخل عددًا صحيحًا.")  # معالجة إدخال غير صحيح
