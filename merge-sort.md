# [Merge Sort](https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar/merge-sort-proje)

### [16,21,11,8,12,22] -> Merge Sort

#### 1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
##### 1. İlk olarak diziyi her elamaın tek başına kalacak şekilde bölüyoruz.
##### 2. Daha sonra elemanları sıralı bir şekilde bir araya getiriyoruz.

|  |  |  |16|21|11|8 |12|22|  |  |  |
|- |- |- |- |- |- |- |- |- |- |- |- |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |16|21|11|  |  |8 |12|22|  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |16|  |21|11|  |  |8 |  |12|22|  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|16|  |21|  |11|  |  |8 |  |12|  |22|
|  |  |  |  |  |  |  |  |  |  |  |  |
|16|  |11|21|  |  |  |8 |  |12|22|  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |11|16|21|  |  |8 |12|22|  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |8 |11|12|16|21|22|  |  |  |

#### 2. Big-O gösterimini yazınız.
##### Merge sort için -> O(nlog(n))