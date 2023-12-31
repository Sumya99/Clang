# Бит хоорондын үйлдлүүд (Bitwise Operators)

Бит хоорондын үндсэн үйлдлүүдэд: AND, OR, XOR, NOT, шилжүүлэх үйлдлүүд орно. ( & | ^ ~ >> << )

<br/> *Дараах хүснэгтүүдэд A,B -ээр битүүдийг, Q -ээр үр дүнг орлуулав* 

1. AND үйлдлийг `&` -ээр тэмдэглэнэ. Аль нэг бит нь 0 бол үр дүн нь 0 болно.

|A|B|Q|
|--	|--|--|
| 0|0 | 0|
| 0|1 | 0|
| 1|0 | 0|
| 1|1 | 1|

2. OR үйлдлийг `|` -ээр тэмдэглэнэ. Аль нэг бит нь 1 бол үр дүн нь 1 болно.

|A|B|Q|
|--	|--|--|
| 0|0 | 0|
| 0|1 | 1|
| 1|0 | 1|
| 1|1 | 1|

3. XOR үйлдлийг `^` -ээр тэмдэглэнэ. Тухайн битүүд нь ялгаатай бол 1 үр дүн гарна. Ижил бол 0 гарна.

|A|B|Q|
|--	|--|--|
| 0|0 | 0|
| 0|1 | 1|
| 1|0 | 1|
| 1|1 | 0|

4. NOT үйлдлийг `~` -ээр тэмдэглэнэ. Өмнөх операторууд 2 битийн хооронд хийгдэж байсан бол NOT нь 1 тоон дээр гүйцэтгэгддэг. 0 -ийг 1, 1-ийг 0 болгоно.

|A|Q|
|--|--|
|0 | 1|
|1 | 0|

5. Баруун тийш шилжүүлэх үйлдлийг `>>` -ээр, зүүн тийш шилжүүлэх үйлдлийг `<<` -ээр тэмдэглэнэ. Дүрэм нь: a<<b, a>>b гэж бичнэ. Энд байгаа a нь шилжүүлэх тоо, b нь хэдэн удаа шилжүүлэх хэмжээ байна.

```c++
Жишээ: 
1. 8 >> 1 үр дүн нь 4 гарна. Яагаад гэвэл 8 = 0b1000 бөгөөд 
үүнийг баруун тийш 1 удаа шилжүүлбэл 0b100 = 4 болно.

2. 1 << 5 үр дүн нь 32 гарна. Яагаад гэвэл 1 = 0b1 бөгөөд 
үүнийг баруун тийш 5 удаа шилжүүлбэл 0b10 0000 = 32 болно.

```
*Тоог нэг удаа баруун тийш шилжүүлэх нь түүнийг хоёрт хуваахтай, зүүн тийш шилжүүлэх нь хоёроор үржихтэй тэнцүү байгааг анзаараарай.*

## Жишээ - Бит хоорондын үйлдлүүд 
```c++
int main()
{
    int a=0b011, b=5; // 5=0b101
    cout<< (a&b)<<'\n'; //1 
    cout<< (a|b)<<'\n'; //7
    cout<< (a^b)<<'\n'; //6
    cout<< (~b)<<'\n'; //-6
    cout<< (1<<b)<<'\n'; //32
    cout<< (a>>1)<<'\n'; //1
    return 0;
}
```

## Жишээ - Тооны битийг удирдах
```c++
int main()
{
    int a=0b111011;
	cout<<(a|1<<2)<<endl; //0b111111
    cout<<(a&(~(1<<4)))<<endl; //0b101011
    return 0;
}
```

## Бие даах дасгалууд

<br/>1. Бит хоорондын үйлдэл ашиглан гараас өгсөн бүхэл тоог тэгш эсэхийг шалга. Тэгш бол Even, сондгой бол Odd гэж хэвлэнэ.
<br/> 12
<br/> Even
<br/> 35
<br/> Odd

<br/>2. XOR үйлдэл ашиглан гараас өгсөн 2 бүхэл тоог тэнцүү эсэхийг шалга. Тэнцүү бол Yes, үгүй бол No гэж хэвлэнэ.
<br/> 789 789
<br/> Yes
<br/> 35 23
<br/> No

<br/>3. Өмнөх дасгалыг AND болон NOT үйлдэл ашиглан гүйцэтгэ.
<br/> 789 789
<br/> Yes
<br/> 35 23
<br/> No

<br/>4. Гараас 0<=n<=40 тоо өгнө. 2^n зэргийг бит хоорондын үйлдлээр ол.
<br/> 10
<br/> 1024
<br/>
<br/> 40
<br/> 1,099,511,627,776

<br/>5. Гараас өгсөн a тооны n дэх битийг set(1 болгох) хийж хэвлэ.
<br/> 1024 0
<br/> 1025
<br/>
<br/> 1024 1
<br/> 1026
<br/>
<br/> 3456 10
<br/> 3456

<br/>6. Гараас өгсөн a тооны n дэх битийг Reset(0 болгох) хийж хэвлэ.
<br/> 1024 4
<br/> 1024
<br/>
<br/> 3456 10
<br/> 2432

<br/>7. Гараас өгсөн a тооны n дэх битийг toggle хий(0 байсан бол 1, 1 байсан бол 0 болгох).
<br/> 3456 10
<br/> 2432
<br/>
<br/> 1024 4
<br/> 1040
