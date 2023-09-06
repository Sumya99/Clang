# Арифметик операторууд 

Арифметик операторууд: 
</p>+ (Нэмэх үйлдэл)
</p>- (Хасах үйлдэл)
</p>* (Үржих үйлдэл) 
</p>/ (Бүхэл хуваах үйлдэл)
</p>% (Бутархай хуваах үйлдэл)

### Жишээ1
```c
int main() {
    int a,b;
    a=18;
    b=10;

    int nemeh;
    int hasah;
    int urjih;
    int buhel_huvaah;
    int butar_huvaah;

    nemeh = a+b;
    hasah = a-b;
    urjih = a*b;
    buhel_huvaah = a/b;
    butar_huvaah = a%b;

    printf("a+b = %d\n",nemeh); //28 garna
    printf("a-b = %d\n",hasah); //8 garna
    printf("a*b = %d\n",urjih); //180 garna
    printf("a/b = %d\n",buhel_huvaah); //1 garna
    printf("a%b = %d\n",butar_huvaah); //8 garna

    return 0;
}
```

### Жишээ2
```c
int main() {
    int a,b;
    a=30;
    b=5;

    int nemeh;
    int hasah;
    int urjih;
    int buhel_huvaah;
    int butar_huvaah;

    nemeh = a+b;
    hasah = a-b;
    urjih = a*b;
    buhel_huvaah = a/b;
    butar_huvaah = a%b;

    printf("a+b = %d\n",nemeh); //35 garna
    printf("a-b = %d\n",hasah); //25 garna
    printf("a*b = %d\n",urjih); //150 garna
    printf("a/b = %d\n",buhel_huvaah); //6 garna
    printf("a%b = %d\n",butar_huvaah); //0 garna

    return 0;
}
```

#Нэг хувьсагчид оператор хэрэглэх

###Жишээ1
```c
int main() {
    int a;
    a=30; // a huvisagchiin utga

    a = a+10;
    a = a-10;
    a = a*10;
    a = a/10;
    a = a%10;

    printf("%d = a+10 \n",a); //40 garna
    printf("%d = a-10 \n",a); //20 garna
    printf("%d = a*10 \n",a); //300 garna
    printf("%d = a/10 \n",a); //3 garna
    printf("%d = a%10 \n",a); //0 garna

    return 0;
}

###Жишээ2 - товчлол

a хувьсагчийн утгыг 10 -аар нэмэгдүүлэх бол өмнөх жишээнд бичснээр a=a+10; гэж бичихэд хангалттай. Тэгвэл үүнийг илүү товчоор a+=10; гэж бичиж болдог. Бусад - * / % операторуудын хувьд ч адил товчлол ашиглаж болно.

```c
int main() {
    int a;
    a=30; // a huvisagchiin utga

    a +=10;
    printf("a = %d \n",a); 
    
    a -=10;
    printf("a = %d \n",a); 
    
    a *=10;
    printf("a = %d \n",a); 
    
    a /=10;
    printf("a = %d \n",a); 
    
    a %=10;
    printf("a = %d \n",a); 
    
    return 0;
}



### Жишээ3 - товчлол
```c
int main() {
    int a,b;
    a=30;
    b=5;

    a = a+b;
    printf("a = %d \n",a);
    a = a-b;
    printf("a = %d \n",a);
    a = a*b;
    printf("a = %d \n",a);
    a = a/b;
    printf("a = %d \n",a);
    a = a%b;
    printf("a = %d \n",a);

    return 0;
}



```
**Гаралт :** 

One Two Three Four
