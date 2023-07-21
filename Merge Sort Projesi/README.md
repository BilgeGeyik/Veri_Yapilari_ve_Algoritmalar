# Project 2

[16,21,11,8,12,22] -> Merge Sort

* Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

* Big-O gösterimini yazınız.

----------------------
**Cevap:** Merge Sort bir listeyi her adımda parçaya ayırıp tek eleman kalıncaya kadar bölüyor. İlk başta sayıyı ikiye böler. Kalan sayı dizsininde ikiye böler. Bu işlem ne zamanki tek bir elaman kalana kadar bölünme işlemi devam eder.

Bundan sonra birleştirme aşaması başlıyor. Birleştirirken sıralama yapılır. Her seferinde elimizde küçük sıralı diziler oluşur.


                  [16,21,11,8,12,22] 

            [16,21,11]        [8,12,22] 
       
        [16,21]  [11]           [8,12]  [22]  
      
      [16] [21] [11]              [8] [12] [22]
    
       [16,21]  [11]              [8,12]  [22]
       
         [11,16,21]               [8,12,22]
       
                  [8,11,12,16,21,22]

    

Merge Sort'un Big-O gösterimi O(n log n) olarak ifade edilir. Tüm sayı dizisine "n" diyelim.

Birleştirme zamanında n  kadar işlem yapılacağı için "O(n)" olarak hesaplanır.

Bölme aşamasında 2^x = n  kadar işlem yapılacağı için "O(logn)" olarak hesaplanır.
