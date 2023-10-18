# Veri_Yapilari_ve_Algoritmalar

## Soru 1

#### [22,27,16,2,18,6]

* Yukarıda verilen diziyi Insertion Sort ile sıralayınız.
```
- [22,27,16,2,18,6] -> 22 en solda olduğu için sıralama yapılmadı
- [22,27,16,2,18,6] -> 27 sayısı bir solundaki 22 sayısından büyük olduğu için yerinde kaldı
- [22,16,27,2,18,6] -> 16 sayısı 27'den küçük olduğu için yerdeğiştirdi
- [16,22,27,2,18,6] -> 16 sayısı 22'den küçük olduğu için yerdeğiştirdi
- [16,22,2,27,18,6] -> 2 rakamı 27'den küçük olduğu için yerdeğiştirdi
- [16,2,22,27,18,6] -> 2 rakamı 22'den küçük olduğu için yerdeğiştirdi
- [2,16,22,27,18,6] -> 2 rakamı 16'dan küçük olduğu için yerdeğiştirdi
- [2,16,22,18,27,6] -> 18 sayısı 27'den küçük olduğu için yerdeğiştirdi
- [2,16,18,22,27,6] -> 18 sayısı 22'den küçük olduğu için yerdeğiştirdi
- [2,16,18,22,6,27] -> 6 rakamı 27'den küçük olduğu için yerdeğiştirdi
- [2,16,18,6,22,27] -> 6 rakamı 22'den küçük olduğu için yerdeğiştirdi
- [2,16,6,18,22,27] -> 6 rakamı 18'den küçük olduğu için yerdeğiştirdi
- [2,6,16,18,22,27] -> 6 rakamı 16'dan küçük olduğu için yerdeğiştirdi
```

* Big-O gösterimini yazınız.
```
n+(n-1)+(n-2)+(n-3)+(n-4)+1 = (n(n+1))/2 = n^2
Big-O = O(n^2)
```

* Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?
  * Average case: Aradığımız sayının ortada olması
  * Worst case: Aradığımız sayının sonda olması
  * Best case: Aradığımız sayının dizinin en başında olması
```
Dizinin sıralı hali [2, 6, 16, 18, 22, 27] şekilindedir. Dolayısıyla 18 average case kapsamındadır.
```

* [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.
```
- [2,3,5,8,7,9,4,15,6] -> Dizideki en küçük eleman (2) bulunur ve en başa alınır.
- [2,3,4,8,7,9,5,15,6] -> Sıradaki en küçük eleman bulunur (3) ve ikinci sıraya yerleştirilir.
- [2,3,4,5,7,9,8,15,6] -> Sıradaki en küçük eleman bulunur (4) ve üçüncü sıraya yerleştirilir.
- [2,3,4,5,6,9,8,15,7] -> Sıradaki en küçük eleman bulunur (5) ve dördüncü sıraya yerleştirilir.
```
