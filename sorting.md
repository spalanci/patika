Proje 1

[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması.
.



[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.


*******

Cevap:

Proje 1 Çözümü
1. Insertion Sort Aşamaları
Dizi: [22, 27, 16, 2, 18, 6]

Insertion Sort, her adımda bir sonraki elemanı alıp, solundaki sıralı kısımda doğru konuma yerleştirir.

Başlangıç: [22, 27, 16, 2, 18, 6]

1. Adım (27): 27, 22'den büyük olduğu için yerinde kalır.
→ [22, 27, 16, 2, 18, 6]

2. Adım (16): 16, 27 ve 22'den küçük; en başa yerleşir.
→ [16, 22, 27, 2, 18, 6]

3. Adım (2): 2, tüm elemanlardan küçük; en başa yerleşir.
→ [2, 16, 22, 27, 18, 6]

4. Adım (18): 18, 27 ve 22'den küçük, 16'dan büyük; 16 ile 22 arasına girer.
→ [2, 16, 18, 22, 27, 6]

5. Adım (6): 6, 16'dan küçük, 2'den büyük; 2 ile 16 arasına girer.
→ [2, 6, 16, 18, 22, 27]

Sonuç: [2, 6, 16, 18, 22, 27]

2. Big-O Gösterimi
Insertion Sort'un zaman karmaşıklığı:

Worst case: O(n²)

Average case: O(n²)

Best case: O(n) — dizi zaten sıralıysa

Verilen dizi için genel Big-O gösterimi: O(n²)

3. Time Complexity — 18 Sayısı
Dizi sıralandıktan sonra: [2, 6, 16, 18, 22, 27]

18 sayısı dizinin 3. indeksinde (0'dan sayarsak) yer alıyor. Dizinin tam ortasında değil ama başta da değil, sonda da değil. 6 elemanlı bir dizide ortadaki konumlar 2. ve 3. indekslerdir (16 ve 18). Bu durumda 18, dizinin ortasına yakın bir konumdadır.

Ancak sorudaki case tanımlarına bakalım:

Average case: Aradığımız sayının ortada olması

Worst case: Aradığımız sayının sonda olması

Best case: Aradığımız sayının dizinin en başında olması

18 sayısı dizinin ortasında (3. indeks, 6 elemanlı dizide ortaya yakın) yer aldığı için Average case kapsamına girer.

Cevap: Average case

4. Selection Sort — İlk 4 Adım
Dizi: [7, 3, 5, 8, 2, 9, 4, 15, 6]

Selection Sort, her adımda dizinin sıralanmamış kısmındaki en küçük elemanı bulup, sıralanmamış kısmın başındaki elemanla yer değiştirir.

Başlangıç: [7, 3, 5, 8, 2, 9, 4, 15, 6]

1. Adım: En küçük eleman: 2 (indeks 4). 2 ile 7 (indeks 0) yer değiştirir.
→ [2, 3, 5, 8, 7, 9, 4, 15, 6]

2. Adım: Kalan kısımda [3, 5, 8, 7, 9, 4, 15, 6] en küçük: 3 (indeks 1). Zaten yerinde.
→ [2, 3, 5, 8, 7, 9, 4, 15, 6]

3. Adım: Kalan kısımda [5, 8, 7, 9, 4, 15, 6] en küçük: 4 (indeks 6). 4 ile 5 (indeks 2) yer değiştirir.
→ [2, 3, 4, 8, 7, 9, 5, 15, 6]

4. Adım: Kalan kısımda [8, 7, 9, 5, 15, 6] en küçük: 5 (indeks 6). 5 ile 8 (indeks 3) yer değiştirir.
→ [2, 3, 4, 5, 7, 9, 8, 15, 6]

İlk 4 adım sonucu: [2, 3, 4, 5, 7, 9, 8, 15, 6]
