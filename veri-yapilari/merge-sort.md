# Merge Sort
---

Bu algoritma diziyi ardışık olarak en küçük alt dizilere yarılar ve tek bir eleman kalana kadar bu işleme devam eder. Tek kalan elemanları birbirleri ile karşılaştırarak tekrar birleştiren algoritmadır.

```
 [16,21,11,8,12,22] 
```

Bu dizi aşağıdaki şemada olduğu gibi sıralanır.

![Merge Sort](/veri-yapilari/img/merge-sort.PNG)

## Big O Gösterimi

* Diziyi parçalara ayırırken sürekli yarıladık yani 2'ye böldük. 
```
2^x=n ==> logn
```
olur.

* Bölünmüş diziyi birleştirirken dizinin uzunluğu olan n kadar birleştirme işlemi yapılır.

```
O(n.logn)
```
sonucuna ulaşırız. Bizim dizimiz 6 elemanlı olduğu için aşağıdaki sonuç 

```
6.log6 
```
olur.
