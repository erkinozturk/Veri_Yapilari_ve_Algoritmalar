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
O(n^2)
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

## Soru 2

#### [16,21,11,8,12,22]

* Yukarıdaki diziyi Merge Sort ile sıralayınız.
```
          [16,21,11]                            [8,12,22]
         /          \                          /         \
     [16,21]    -    [11]                 [8,12]    -    [22]
    /       \            \               /      \            \
 [16]    -   [21]    -    [11]        [8]    -   [12]    -    [22]   
     \      /              /             \      /            /
     [16,21]     -     [11]               [8,12]     -    [22]
            \          /                        \        /
             [11,16,21]                          [8,12,22]
                         \                      /
                            [8,11,12,16,21,22]
```

* Big-O gösterimini yazınız.
```
O(nlogn)
```

## Soru 3

* [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
```
Root = 7
              7
            /   \
          5       8
        /   \       \
       1     6        9
     /   \
   0      3
        /   \
      2       4

Root'u 7 aldık. 7'den büyük olan rakamları 7'nin sağına, küçük olan rakamları soluna yazıp, her dalda bu işlemi uygulayarak bir ağaç oluşturduk.
```
