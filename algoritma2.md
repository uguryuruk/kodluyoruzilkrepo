# Merge Sort Projesi

## Proje 2
[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.

## CEVAP

1. [16,21,11,8,12,22] -> Orjinal

* Parçalama aşaması:
* [16,21,11] ------ [8,12,22]
* [16,21]--[11] ------ [8,12]--[22]
* [16]--[21]--[11] ------ [8]--[12]--[22]
* birleştirme aşaması başlar:
* [16,21]--[11] ------ [8,12]--[22]
* [11,16,21] ------ [8,12,22]
* [8,11,12,16,21,22] 

2. Big O gösterimi, bütün elemanları tek tek dolaşmayacağı ve parçaladıktan sonra birleştirirken en küçükleri karşılaştırarak gidecektir. Her bölünmüş dizinin Merge işlemi için de dizinin uzunluğu olan n işlem yapıldığından  O(n*(log<sub>n</sub>))=  O(6*(log<sub>6</sub>))olacaktır.
