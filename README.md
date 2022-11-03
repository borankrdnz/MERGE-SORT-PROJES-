# [Patika.dev](https://www.patika.dev/tr)

# MERGE-SORT-PROJESI-
[16,21,11,8,12,22] -> Merge Sort  Yukarıdaki dizinin sort türüne göre aşamalarını yazınız. Big-O gösterimini yazınız.
-----------------------------------------------------------------------


   [16, 21, 11, 8, 12, 22] dizisinin Merge Sort'a göre adımları;

   Diziyi tek eleman kalıncaya kadar ikili parçalara ayırmamzı gerekmektedir.
    [16, 21, 11] --- [8, 12, 22]
    [16] --- [21, 11] --- [8] --- [12, 22]
    [16] --- [21] +++ [11] --- [8] --- [12] +++ [22]

   Birleştirme işlemine sayısal değeri küçük olan elemanla başlamalıyız.;
    [16] --- [11, 21] --- [8] --- [12, 22]
    [11, 16, 21] --- [8, 12, 22]

    [8, 11, 12, 16, 21, 22]

    Big O gösterimi;

    Diziyi parçalara ayırırken sürekli 2'ye böldüğümüz için; 2^x = n => logn
    Elemanların birbirlerine göre karşılaştırması; n - 1 => n
    Bütun bu işlemlerin sonucu; O(n * logn)
