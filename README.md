# patika.dev Merge Sort Project  
Proje 2  
[16,21,11,8,12,22] -> Merge Sort  

# Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.  

 Merge Sort listeyi her adımda iki parçaya ayırıp tek eleman kalıncaya kadar bölüyor. Böldükten sonra sıralı bir şekilde bize sunuyor.  
 # Önce tek eleman kalana kadar bölelim.

1. [16,21,11,8,12,22] =>     [16,21,11] / [8,12,22]  

2. [16,21,11] => [16,21] / [11]   
   [8,12,22]  => [8,12] / [22]  
   
3. [16,21] / [11] => [16] / [21] / [11]  
   [8,12] /  [22] => [8] / [12] / [22]  
   
# Sonra da en küçük elemanları en başa alıp küçükten büyüğe doğru sıralayalım.  

4. [16] /[21] / [11] => [11,16,21]  
   [8] / [12] / [22] => [8,12,22]   
   
# Şimdi en başta ikiye böldüğümüz diziyi küçükten büyüğe doğru birleştiriyoruz.    
 
5. [8,11,12,16,21,22]  

#  ÖZETLE   
                                      [16,21,11,8,12,22]  
                                       /              \
                                   [16,21,11]     [8,12,22]
                                     /                  \ 
                             [16]  [21,11]         [8,12]  [22]
                                  /                       \
                         [16] [21] [11]                  [8] [12] [22]
                                   \                       /
                                  [11,16,21]          [8,12,22]
                                      \                 /
                                       [8,11,12,16,21,22]
                               

        
# Big-O gösterimini yazınız.    
         O(n.logn)  
         
# www.patika.dev         
