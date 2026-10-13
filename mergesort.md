Proje 2

[16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.
********************

Proje 2 Çözümü
1. Merge Sort Aşamaları
Dizi: [16, 21, 11, 8, 12, 22]

Merge Sort, diziyi sürekli ikiye bölerek tek elemanlı alt diziler oluşturur, sonra bunları sıralı şekilde birleştirir.

Bölme (Divide) Aşaması
Seviye 0:
[16, 21, 11, 8, 12, 22]

Seviye 1:
[16, 21, 11] — [8, 12, 22]

Seviye 2:
[16, 21] — [11] — [8, 12] — [22]

Seviye 3:
[16] — [21] — [11] — [8] — [12] — [22]

Birleştirme (Merge) Aşaması
Seviye 3 → 2:

[16] ve [21] → [16, 21]

[11] tek başına → [11]

[8] ve [12] → [8, 12]

[22] tek başına → [22]

Durum: [16, 21] — [11] — [8, 12] — [22]

Seviye 2 → 1:

[16, 21] ve [11] → [11, 16, 21]

[8, 12] ve [22] → [8, 12, 22]

Durum: [11, 16, 21] — [8, 12, 22]

Seviye 1 → 0:

[11, 16, 21] ve [8, 12, 22] → [8, 11, 12, 16, 21, 22]

Sonuç: [8, 11, 12, 16, 21, 22]

Adım Adım Özet
Adım	İşlem	Sonuç
1	[16, 21, 11, 8, 12, 22]	Böl
2	[16, 21, 11] — [8, 12, 22]	Böl
3	[16, 21] — [11] — [8, 12] — [22]	Böl
4	[16] — [21] — [11] — [8] — [12] — [22]	Tek elemanlar
5	[16, 21] — [11] — [8, 12] — [22]	Birleştir
6	[11, 16, 21] — [8, 12, 22]	Birleştir
7	[8, 11, 12, 16, 21, 22]	Birleştir (Sonuç)
