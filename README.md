# #  ÖDEV2
#  1)Aldığı isim soy isim ile listeye öğrenci ekleyen.

öğrenciler = ["Nazli İnal","Can Yılmaz","Seda Demir"]
print (öğrenciler)

öğrenciler.append("Tuğba Çelik") 
print(öğrenciler)

#  2) Aldığı isim soy isim ile eşleşen değeri listeden kaldıran.
öğrenciler = ["Nazli İnal","Can Yılmaz","Seda Demir"]
öğrenciler.remove("Nazli İnal")
print(öğrenciler)   

#  3) Listeye birden fazla öğrenci eklemeyi mümkün kılan.
öğrenciler.extend(["Ali Yıldırım","Buse İnce"])
print(öğrenciler)

#  4) Listedeki tüm öğrencileri tek tek ekrana yazdıran.
öğrenciler = ["Nazli İnal","Can Yılmaz","Seda Demir"]
i= 0
for i in range(len(öğrenciler)):
    print(öğrenciler[i])

#  5)Öğrencinin listedeki index numarası öğrenci numarası olarak
#  kabul edildiğini düşünerek öğrencinin numarasını öğrenmeyi mümkün kılan

öğrenciler = ["Nazli İnal","Can Yılmaz","Seda Demir"]
print ("Nazli İnal: ", öğrenciler.index("Nazli İnal"))
print( "Can Yılmaz:",öğrenciler.index ("Can Yılmaz"))
print("Seda Demir:", öğrenciler.index("Seda Demir"))

# 6) Listeden birden fazla öğrenci silmeyi mümkün kılan (döngü kullanınız)

öğrenciler = ["Nazli İnal","Can Yılmaz","Seda Demir"]   
def öğrenciSilme ():
    sayi = input ("Silinecek öğrencinin sayisini giriniz:")
    yeniListe = []
    i = 0
    while i < sayi:
    öğrenciSilme= input("Silinecek öğrencinin adi :")
    i += 1
    yeniListe.append (öğrenciSilme)

    for öğrenci in öğrenciler:
        if öğrenci in yeniListe:
            öğrenciler.remove(öğrenci)
print (öğrenciler)           
