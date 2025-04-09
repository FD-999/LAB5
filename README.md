def massiv_hasilini_hesabla(B):
    hasil = 1  
    tapildi = False  

    for elem in B:
        if elem > 9:
            hasil *= elem
            tapildi = True

    if tapildi:
        return hasil
    else:
        return "9-dan böyük element yoxdur"
n = int(input("Massivin ölçüsünü daxil edin: "))
B = []
print("Massivin elementlərini daxil edin:")
for i in range(n):
    B.append(int(input()))
nəticə = massiv_hasilini_hesabla(B)
print(f"Nəticə: {nəticə}")
