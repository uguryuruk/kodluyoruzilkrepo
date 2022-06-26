# Insertion Sort Projesi

## Proje 1

[22,27,16,2,18,6] -> Insertion Sort

1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


5. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

## CEVAP:

1. Insertion sort, projede adım adım giderek sürekli olarak en küçükleri bulup yer değiştirmek suretiyle çalışır. Böylece kalan değerlerden en küçüğü sürekli bulunup başa getirilerek sıralama yapılır. Aşamaları:
* [22,27,16,2,18,6] : Orjinal durum.
* [**2**,27,16,**22**,18,6] : Minimum değer 2 ile 22 yer değiştirir, sonra dizinin sıradaki elemanına (27) geçilir.
* [2,**6**,16,22,18,**27**] : Kalan değerler arasından Minimum değer 6 ile 27 yer değiştirir, sonra dizinin sıradaki elemanına (16) geçilir.
* [2,6,16,22,18,27] : 16 zaten minimum olduğu için sıradaki elemana geçilir.
* [2,6,16,**18**,**22**,27] : Böylece sıralama tamamlanır.

2. Big O notation n*(n+1)/2 olacağından O(n<sup>2</sup>) olacaktır.

3. Aslında benim görüşüme göre Time Complexity:

* Average case: dizinin yaklaşık sıralı olması,
* Worst case: dizinin ortalama değerler-büyük değerler-küçük değerler şeklinde yığılması,
* Best case: dizinin küçük değerler-ortalama değerler-büyük değerler şeklinde yığılmış olmasıdır.

4. 18 sayısı ortalarda olduğu için average case kapsamına girer.

5. [7,3,5,8,2,9,4,15,6] : Orjinal

* [**2**,3,5,8,**7**,9,4,15,6] 
* [2,3,**4**,8,7,9,**5**,15,6] 
* [2,3,4,**5**,7,9,**8**,15,6] 
* [2,3,4,5,**6**,9,8,15,**7**] 
* [2,3,4,5,6,**7**,8,15,**9**] 
* [2,3,4,5,6,7,8,**9**,**15**] 

