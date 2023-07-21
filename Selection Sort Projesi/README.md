# Proje 1
**[22,27,16,2,18,6]** -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

--------------------------------
**Cevap:** Insertion Sort, sıralama algoritmalarından biridir ve temel olarak bir diziyi küçükten büyüğe doğru sıralamak için kullanılır. 
1. Bu sayı öbeğinin en küçük elemanını bulup onu en baştaki sayı elemanıyla yer değiştilir.

    [2| 27, 16, 22, 18, 6]

2. Baştaki sayının en küçük olduğunu biliyorum.Yanına gelecek sayı öbeğindeki ikinci en küçük elemanı yanındaki sayı ile yer değiştirilir.
  
   [2, 6| 16, 22, 18, 27]

3. Sıralı sayı öbeğindeki (çizginin sol tarafı) ikinci elmanın yanına gelecek üçüncü elaman için sırasız olan sayı öbeğindeki (çizginin sağ tarafı) küçük sayı ile yer değişimi yapılır.

    [2, 6, 16| 22, 18, 27]

    ***NOT:*** *Bu adımda sırasız olan sayı öbeğindeki (çizginin sağ tarafı) küçük sayı 16 olduğu için sayı öbeğinde başka bir sayıla değişim olmadı.*

4.  Çizginin sağ tarafında en küçük sayı seçilir ve 16'nın yanındaki sayı ile yer değiştirilir.

    [2, 6, 16, 18| 22, 27]

5. Çizginin sağ tarafında en küçük sayı seçilir ve 18'nın yanındaki sayı ile yer değiştirilir ve sıralama tamamlanmış olur.

    [2, 6, 16, 18, 22, 27]

-------------------------

Big-O gösterimini yazınız.

--------------------------
**Cevap:** Sayı öbeğine "n" kadar sayı var diyelim. İlk sıralamada n'den başlayarak tüm sıralamalar -1 azalacak. Yani ikinci adımda "n-1" kadar arama yapacak. Üçüncü adımda "n-2" kadar arama yapacak. Bu işlem "1"sayısını bulana kadar devam edecek. 

n + (n-1) + (n-2)... kadar işlem yapılacağı için n.(n+1)/2 şeklinde hesaplanır.

Hesaplamalar sonucunda elde edilen (n2+n)/2 değerinin asimptotik üst sınırı O(n2) değerini verir.

---------------------------

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

1. Average case: Aradığımız sayının ortada olması
2. Worst case: Aradığımız sayının sonda olması
3. Best case: Aradığımız sayının dizinin en başında olması.

----------------
**Cevap:** Average case: Aradığımız sayının ortada olması.

----------------------

**[7,3,5,8,2,9,4,15,6]** dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

-----------------------
**Cevap:**

1. adım
    
    [2| 3, 5, 8, 7, 9, 4, 15, 6]

2. adım

    [2, 3| 5, 8, 7, 9, 4, 15, 6]

3. adım

    [2, 3, 4| 8, 7, 9, 5, 15, 6]

4. adım

    [2, 3, 4, 6| 7, 9, 8, 15, 6]
