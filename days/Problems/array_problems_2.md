# Нэг хэмжээст Array бодлогууд 1

<br>1. Гараас n(100 -аас ихгүй) тоо өгнө. Үүний дараа n ширхэг бүхэл тоо өгнө. 2 дахь болон n-2 дахь элементүүдийн нийлбэрийг хэвлэ.

**Оролт1:** 
<br>10 
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
10

**Оролт2:** 
<br>17 
<br>123 456 789 10 11 12 123 456 789 1157 88 7 6 78 3 78 64

**Гаралт2:**
459


<br>2. Гараас n(100 -аас ихгүй) тоо өгнө. Үүний дараа n ширхэг бүхэл тоо өгнө. n дэх элементэд хуваагддаг бүх элементүүдийг хэвлэ.Элементүүд давтагдаж болно. Хуваагддаг элемент олдохгүй бол -1 хэвлэ.

**Оролт1:** 
<br>10
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
-1

**Оролт2:** 
<br>20
<br>78 4 1 58 2 78 9 1 58 2 78 4 1 58 2 78 4 1 58 3

**Гаралт2:**
78 78 9 78

<br>3. Гараас n(100 -аас ихгүй) ба k тоонууд өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. k тоо хэд дэх индекс дээр байгааг хэвлэ. k тоо олон удаа олдвол бүх индексийг хэвлэ. Хэрэв олдохгүй бол -1 хэвлэ. 

**Оролт1:** 
<br>10 78
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
-1

**Оролт2:** 
<br>10 8
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт2:**
7

**Оролт3:** 
<br>20 58
<br>78 4 1 58 2 78 9 1 58 2 78 4 1 58 2 78 4 1 58 3

**Гаралт3:**
3 8 13 18








<br> <br><br> <br>
## Шинэ бодлогууд

**4.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Array-н элементүүдийг өгсөн дарааллыг урвуугаар хэвлэ. 

**Оролт1:** 
<br>10 </pr>
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
<br>10 9 8 7 6 5 4 3 2 1

**Оролт2:** 
<br>8 </pr>
<br>13 22 33 42 555 346 72 99

**Гаралт2:**
99 72 346 555 42 33 22 13

**5.** Эхлээд n ба k тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Array-н элементүүд дотороос k -ээс бага хамгийн том тоог ол. Үргэлж тийм тоо олдоно гэж тооц.

**Оролт1:** 
<br>10 5</pr>
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
4

**Оролт2:** 
<br>8 400 </pr>
<br>13 22 33 42 555 346 72 99

**Гаралт2:**
346

**6.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Array-н 2 дахь том элементийг хэвлэ.

**Оролт1:** 
<br>10 </pr>
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
9

**Оролт2:** 
<br>8 </pr>
<br>13 22 33 42 555 346 72 99

**Гаралт2:**
346

**7.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Абсолют зөрүү нь нэгтэй тэнцүү хос элементүүдийг шинэ мөрөнд хэвлэ. 

**Оролт1:** 
<br>10 </pr>
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
<br>1 2</pr>
<br>2 3</pr>
<br>3 4</pr>
<br>4 5</pr>
<br>5 6 </pr>
<br>6 7</pr>
<br>7 8 </pr>
<br>8 9</pr>
<br>9 10</pr>

**Оролт2:** 
10 </pr>
13 23 32 4 5 22 7 33 9 11

**Гаралт2:**
<br>23 22</pr>
<br>32 33</pr>

**8.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Хэрэв Array-н элемент тэгш бол тухайн элементэд 0, сондгой 1 утга оноож хэвлэ.  

**Оролт1:** 
<br>10 </pr>
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
1 0 1 0 1 0 1 0 1 0

**Оролт2:** 
<br>10 </pr>
<br>112 32 33333 42 521 61 70 45 90 100
**Гаралт2:**
0 0 1 0 1 1 0 1 0 0


**9.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Array-н ялгаварын абсолют утга нь хамгийн бага байх 2 хос элементийг хэвлэ. Ялгаварын утга нь хамгийн бага тэнцүү олон тохиолдол байвал аль нэгийг нь хэвлэ.
**Оролт1:** 
<br>10 </pr>
<br>1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
1 2   *(2 3, 3 4 ... 9 10 байсан ч болно)*

**Оролт2:** 
<br>10 </pr>
<br>112 32 33333 42 521 61 70 45 90 100
**Гаралт2:**
61 70

**10.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Array-н элементүүдийг өсөх эрэмбээр хэвлэ.

**Оролт1:** 
<br>10 </pr>
<br>12 2 3 422 5 6 7 8 9 11

**Гаралт1:**
2 3 5 6 7 8 9 11 12 422

**Оролт2:** 
<br>8 </pr>
<br>13 22 33 42 555 346 72 99

**Гаралт2:**
13 22 33 42 72 99 346 555

**11.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Array-н элементүүдийг буурах эрэмбээр хэвлэ.

**Оролт1:** 
<br>10 </pr>
<br>12 2 3 422 5 6 7 8 9 11

**Гаралт1:**
422 12 11 9 8 7 6 5 3 2

**Оролт2:** 
<br>8 </pr>
<br>13 22 33 42 555 346 72 99

**Гаралт2:**
555 346 99 72 42 33 22 13

**12.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Нэгээс олон давтагдаж буй Array-н элементийг өсөх дарааллаар хэвлэ.

**Оролт1:** 
<br>10 </pr>
<br>11 2 3 2 7 6 7 7 9 11

**Гаралт1:**
2 7 11

**Оролт2:** 
<br>8 </pr>
<br>13 22 99 99 555 22 72 99

**Гаралт2:**
22 99

**13.** Эхлээд n тоо өгөгдөнө. Үүний дараа n ширхэг бүхэл тоо өгнө. Давтагдаагүй Array-н элементүүдийг өсөх дарааллаар хэвлэ.

**Оролт1:** 
<br>10 </pr>
<br>11 2 3 2 7 6 7 7 9 11

**Гаралт1:**
3 6 9 

**Оролт2:** 
<br>10 </pr>
<br>13 22 99 99 555 22 72 99 1000 1001

**Гаралт2:**
13 72 555 1000 1001


<!-- 
11.Эхлээд n тоо өгөгдөнө. Үүний дарааа n ширхэг бүхэл тоо өгнө. Array-н элементүүдээс анхны тоонуудыг хасаж үлдсэнийг нь хэвлэ.

**Оролт1:** 
10 </pr>
1 2 3 4 5 6 7 8 9 10

**Гаралт1:**
1 4 6 8 9 10

**Оролт2:** 
8 </pr>
13 22 33 42 555 346 72 99

**Гаралт2:**
22 33 42 555 346 72 99 -->
<!-- Хүснэгтийн элементүүдийн нийлбэрийг олох функц бичих.
Хүснэгтийн элементүүдийн нийлбэрийг олох рекурсив функц бичих.
Хүснэгтийн элементүүдийн хамгийн том тоог олох рекурсив функц бичих.
 -->


