Soru: [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
*******************************************************
Çözüm:
Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.
Binary Search Tree (BST) Aşamaları
Dizi: [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

BST kuralı: Her düğüm için, solundaki tüm değerler kendisinden küçük, sağındaki tüm değerler kendisinden büyük olmalıdır. İlk eleman root olarak alınır.

Adım Adım Ekleme
1. Eleman: 7 → Root

text
        7
2. Eleman: 5 → 5 < 7, root'un soluna gider.

text
        7
       /
      5
3. Eleman: 1 → 1 < 7 (sola), 1 < 5 (sola).

text
        7
       /
      5
     /
    1
4. Eleman: 8 → 8 > 7, root'un sağına gider.

text
        7
       / \
      5   8
     /
    1
5. Eleman: 3 → 3 < 7 (sola), 3 < 5 (sola), 3 > 1 (sağa).

text
        7
       / \
      5   8
     /
    1
     \
      3
6. Eleman: 6 → 6 < 7 (sola), 6 > 5 (sağa).

text
        7
       / \
      5   8
     / \
    1   6
     \
      3
7. Eleman: 0 → 0 < 7 (sola), 0 < 5 (sola), 0 < 1 (sola).

text
        7
       / \
      5   8
     / \
    1   6
   / \
  0   3
8. Eleman: 9 → 9 > 7 (sağa), 9 > 8 (sağa).

text
        7
       / \
      5   8
     / \   \
    1   6   9
   / \
  0   3
9. Eleman: 4 → 4 < 7 (sola), 4 < 5 (sola), 4 > 1 (sağa), 4 > 3 (sağa).

text
        7
       / \
      5   8
     / \   \
    1   6   9
   / \
  0   3
       \
        4
10. Eleman: 2 → 2 < 7 (sola), 2 < 5 (sola), 2 > 1 (sağa), 2 < 3 (sola).

text
        7
       / \
      5   8
     / \   \
    1   6   9
   / \
  0   3
     / \
    2   4
Son BST Yapısı
text
            7
           / \
          5   8
         / \   \
        1   6   9
       / \
      0   3
         / \
        2   4
Özet (Adım Adım Yol)
Eleman	Karşılaştırma Yolu	Konum
7	—	Root
5	7'nin soluna	7'nin solu
1	7 sol → 5 sol	5'in solu
8	7'nin sağına	7'nin sağı
3	7 sol → 5 sol → 1 sağ	1'in sağı
6	7 sol → 5 sağ	5'in sağı
0	7 sol → 5 sol → 1 sol	1'in solu
9	7 sağ → 8 sağ	8'in sağı
4	7 sol → 5 sol → 1 sağ → 3 sağ	3'ün sağı
2	7 sol → 5 sol → 1 sağ → 3 sol	3'ün solu
