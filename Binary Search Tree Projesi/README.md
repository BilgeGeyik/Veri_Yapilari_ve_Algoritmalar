# Project 3

**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]** dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

--------------------------
**Cevap:** Binary Search Tree, her düğümde sol alt ağacın tüm değerlerinin düğüm değerinden küçük, sağ alt ağacın tüm değerlerinin ise düğüm değerinden büyük olduğu bir ağaç yapısıdır.

1. Root ilk elamını root olarak alırız.
            
            7

2. Dizideki ikinci elemana bakılır. 5<7 ; root'un sol tarafına 5 eklenir.

           7
         /
       5 

3. Dizideki bir sonraki elemana bakılır. 1<7 ; root'un sol tarafındaki düğüme yönlendirilir.
1<5; 5'in sol tarafına eklenir.

                7
              /
            5 
          / 
        1 

4. Dizideki bir sonraki elemana bakılır. 8>7 ; root'un sağ tarafına eklenir.

                7
              /   \
            5       8
          / 
        1 

5. Dizideki bir sonraki elemana bakılır. 3<7 ; root'un sol tarafındaki birinci düğüme yönlendirilir. 3<5; sol tarafındaki ikinci düğüme yönlendirilir. 3>1 ; 1'in sağ tarafına eklenir.

                7
              /   \
            5       8
          / 
        1 
          \
            3

6. Dizideki bir sonraki elemana bakılır. 6<7 ; root'un sol tarafındaki birinci düğüme yönlendirilir. 6>5; 5'in sağ tarafına eklenir.

                7
              /   \
            5       8
          /   \
        1       6
          \
            3
 
 6. Dizideki bir sonraki elemana bakılır. 0<7 ; root'un sol tarafındaki birinci düğüme yönlendirilir. 0<5; sol tarafındaki ikinci düğüme yönlendirilir. 0<1 ; 1'in sol tarafına eklenir.

                   7
                 /   \
               5       8
             /   \
           1       6
          /  \
        0      3
 
 7. Dizideki bir sonraki elemana bakılır. 9<7 ; root'un sağ tarafındaki birinci düğüme yönlendirilir. 9<8; 8'in sağ tarafına eklenir.

                   7
                 /   \
               5       8
             /   \       \
           1       6       9
          /  \
        0      3

8. Dizideki bir sonraki elemana bakılır. 4<7 ; root'un sol tarafındaki birinci düğüme yönlendirilir. 4<5; sol tarafındaki ikinci düğüme yönlendirilir. 4>1 ; 1'in sağ tarafındaki düğüme yönlendirilir. 4>3; 3^ün sağ tarafına eklenir.

                   7
                 /   \
               5       8
             /   \       \
           1       6       9
          /  \
        0      3
                \
                  4

9. Dizideki bir sonraki elemana bakılır. 2<7 ; root'un sol tarafındaki birinci düğüme yönlendirilir. 2<5; sol tarafındaki ikinci düğüme yönlendirilir. 2>1 ; 1'in sağ tarafındaki düğüme yönlendirilir. 2<3; 3^ün sol tarafına eklenir.

                   7
                 /   \
               5       8
             /   \       \
           1       6       9
          /  \
        0      3
              /  \
            2      4
