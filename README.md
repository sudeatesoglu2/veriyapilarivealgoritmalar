## PROJECT-1
# Selection Sort

[patika profil](https://app.patika.dev/sudeatesoglu)
<br>
[patika.dev link](https://app.patika.dev/)
---

[22,27,16,2,18,6] -> selection sort

1. Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.

|1. adım|2|27|16|22|18|6|
|-------|-|- |- |- |- |-|
|2. adım|2|6 |16|22|18|27|
|3. adım|2|6 |16|18|22|27|

2. Big-O gösterimini yazınız.

işlem sayısı => n*(n+1)/2 (n^2+n)/2 --> **big-o gösterimi** => O(n^2)

3. Time Complexity:

Best case: Aradığımız sayının dizinin en başında olması. <br>
Average case: Aradığımız sayının ortada olması. <br>
Worst case: Aradığımız sayının sonda olması.

4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.

sıralanmış dizide ortadaki elemandır; **average case** kapsamına girer.

5. [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

|1. adım|2|3|5|8|7|9|4|15|6|
|-------|-|-|-|-|-|-|-|- |-|
|2. adım|2|3|4|8|7|9|5|15|6|
|3. adım|2|3|4|5|7|9|8|15|6|
|4. adım|2|3|4|5|6|9|8|15|7|

## PROJECT-2
# Merge Sort
[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

|  |  |  |  |  |  |  |  |  |  |  |  |
|- |- |- |- |- |- |- |- |- |- |- |- |
|  |  |  |16|21|11|8 |12|22|  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |16|21|11|  |  |8 |12|22|  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |16|21|  |11|  |  |8 |  |12|22|  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|16|  |21|  |11|  |  |8 |  |12|  |22|
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |16|21|  |11|  |  |8 |  |12|22|  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |11|16|21|  |  |8 |12|22|  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |8 |11|12|16|21|22|  |  |  |
    
2. Big-O gösterimini yazınız.

O(n*logn) => O(6*log6)

## PROJECT-3
# Binary-Search-Tree

1. [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

root 7dir
5<7; rootun solunda bulunur.

|  |  |  |
|- |- |- |
|  |7 |  |
|5 |  |  |

1<7 ve 1<5;
|  |  |  |  |
|- |- |- |- |
|  |  |7 |  |
|  |5 |  |  |
|1 |  |  |  |

8>7; rootun sağında bulunur.
|  |  |  |  |
|- |- |- |- |
|  |  |7 |  |
|  |5 |  |8 |
|1 |  |  |  |

3<7, 3<5, 3>1;
|  |  |  |  |
|- |- |- |- |
|  |  |7 |  |
|  |5 |  |8 |
|1 |  |  |  |
|  |3 |  |  |

6<7, 6>5;
|  |  |  |  |  |
|- |- |- |- |- |
|  |  |7 |  |  |
|  |5 |  |8 |  |
|1 |  |6 |  |  |
|  |3 |  |  |  |

0<7, 0<1;
|  |  |  |  |  |  |
|- |- |- |- |- |- |
|  |  |  |7 |  |  |
|  |  |5 |  |8 |  |
|  |1 |  |6 |  |  |
|0 |  |3 |  |  |  |

9>7, 9>8;
|  |  |  |  |  |  |
|- |- |- |- |- |- |
|  |  |  |7 |  |  |
|  |  |5 |  |8 |  |
|  |1 |  |6 |  |9 |
|0 |  |3 |  |  |  |

4<7, 4<5, 4>1;
|  |  |  |  |  |  |
|- |- |- |- |- |- |
|  |  |  |7 |  |  |
|  |  |5 |  |8 |  |
|  |1 |  |6 |  |9 |
|0 |  |3 |  |  |  |
|  |  |  |4 |  |  |

2<7, 2<5, 2>1, 2<3;
|  |  |  |  |  |  |  |  |
|- |- |- |- |- |- |- |- |
|  |  |  |  |7 |  |  |  |
|  |  |  |5 |  |8 |  |  |
|  |  |1 |  |6 |  |9 |  |
|  |0 |  |3 |  |  |  |  |
|  |  |2 |  |4 |  |  |  |
