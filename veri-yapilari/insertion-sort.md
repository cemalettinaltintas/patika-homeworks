# Insertion Sort Projesi

Insertion sort sıralı diziyi her adımda eleman eleman oluşturan bir sıralama algoritmasıdır. Düzensiz dizi elemanlarını tek tek ele alarak her birini sıralanmış kısmındaki uygun yerine yerleştirme esasına dayanır.

Başta dizinin 2. elemanı seçilir ve öndeki elemanla karşılaştırma yapılır, eğer önündeki elemandan küçükse yer değiştirirler. Bu işlem sonunda 3. eleman seçilir ve öndeki elemanlarla karşılaştırma yapılır, önündeki elemanlardan küçükse yer değiştirme işlemi yapılır. Dizinin sonunda gelene kadar bu algoritma mantığı devam eder.

## Örnek
``` 
[22,27,16,2,18,6] 
```

Bu diziyi insertion sort algoritması ile sıralama işlemi yapacağız.

![Insertion Sort](img/insertion-sort.PNG)

## C# Kodları:

```c#
        static void Main(string[] args)
        {
             int[] dizi = { 22, 27, 16, 2, 18, 6 };
             sirala(dizi);
        }
        static void sirala(int[] dizi)
        {
            int n = dizi.Length,deger,j;
            
            for (int i = 1; i <n; i++)
            {
                deger = dizi[i];
                j = i - 1;
                while (j>=0 && dizi[j]>deger)
                {
                    dizi[j + 1] = dizi[j];
                    j--;
                }
                dizi[j + 1] = deger;
            }
        }

```