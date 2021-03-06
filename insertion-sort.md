# [Insertion Sort](https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar/insertion-sort-proje)
### [22,27,16,2,18,6] -> Insertion Sort

##### 1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Algoritma her seferinde dizinin elemanlarını öncesindeki elemanlar ile karşılaştırarak, büyük elemanları bir sağa kaydırarak ilerler. Daha büyük bir eleman kalmadığında eleman son kaydırılan elemanın yerini alır.
   
1 - İlk olarak 22 sayısı ile başlarız ve elimizdeki tek eleman olduğu için sonraki sayı ile devam ederiz.
|22|27|16|2|18|6|     
|- |- |- |-|- |-|
    
2 - Sıradaki 27 sayısı ile öncesindeki 27'yi karşılaştırırız. 22, 27 küçük olduğu için değişiklik yapmadan devam ederiz.
|22|27|16|2|18|6|     
|- |- |- |-|- |-|
    
3 - Sıradaki 16 sayısı ile gerisindeki sayıları kıyaslarız. 16 hem 27'den hem de 22'den küçük olduğu için bu iki sayı bir sağa kaydırılır ve 16 en başa geçer.\
|16| | | | | | | | | | | | |
|- |-|-|-|-|-|-|-|-|-|-|-|-|
|&darr;| | |  | | | | | | | | | |
|  |22|27|2|18|6|-->|16|22|27|2|18|6| 

       
4 - 2 ile bir gerisindeki sayılar birer birer karşılaştırılır. 2 27'den küçük olduğu için 27 bir sağa kayar. Aynı şekilde 22 ve 16 da 2'den küçük olduğundan sağa kaydırılır ve 2 en başa geçer.
|16|22|  |27|18|6|->|16|  |22|27|18|6|->|  |16|22|27|18|6| 
|- |- |- |- |- |-|--|- |- |- |- |- |-|--|- |- |- |- |- |-|

|2     | | | | | |
|- |- |- |- |- |-|
|&darr;| | | | | |
|  |16|22|27|18|6|

    
5 - 18 ile gerisindeki 27'yi karşılaştırırız. 18 27'den küçük olduğundan 27 bir sağa geçer. Aynı şekilde 22 de bir sağa kaydırılır. 16 18'den küçük olduğundan 18 22'nin eski yerini alır.
|2 |16|22| |27|6|-->|2|16|  |22|27|6|
|- |- |- |-|- |-|---|-|- |- |- |- |-|

| |  |18|  |  | |
|-|- |- |- |- |-|
| |  |&darr;| |||
|2|16|  |22|27|6|

   
6 - 6 ile bir gerisindeki sayıyı kıyaslanır. 6 27-22-18-16 sayılarından küçük olduğu için bu sayılar sırası ile bir sağa kaydırılır. 6 2'den büyük olduğundan son kaydırılan 16'nın yerini alır.
|2 |16|18|22|- |27|-->|2 |16|18| |22|27|-->|2 |16|- |18|22|27|
|- |- |- |- |- |- |---|- |- |- |-|- |- |---|- |- |- |- |- |- |
    
|-->|2 |- |16|18|22|27|
|---|- |- |- |- |- |- |

| |6     | | | | |
|-|-     |-|-|-|-|
| |&darr;| | | | |
|2|  |16|18|22|27|

##### 2. Big-O gösterimini yazınız.
Insertion sort için -> O(n^2)

##### 3. Time Complexity: 
###### - Worst case: Aradığımız sayının sonda olması

###### - Average case: Aradığımız sayının ortada olması

###### - Best case: Aradığımız sayının dizinin en başında olması

##### 4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
18 elimizdeki listede orta sıralarda olduğu için **average case** diyebiliriz.
    
#### 2. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
1.
|7|3|5|8|2|9|4|15|6|      
|-|-|-|-|-|-|-|- |-|
2.
|3| | | | | | |  | |
|-|-|-|-|-|-|-|- |-|
|&darr;| | | | | ||||
|  |7|5|8|2|9|4|15|6|      

3.
| |5| | | | | |  | |
|-|-|-|-|-|-|-|- |-|
||&darr;| | | | | |||
|3| |7|8|2|9|4|15|6|

4.
|3|5|7|8|2|9|4|15|6|      
|-|-|-|-|-|-|-|- |-|
 