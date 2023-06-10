# Operador de Nivel de Bits

### El operador and "&" 

```c++
void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  int num = 4; //100 en binario
  int num2 = 5; //101 en binario

  //Retardo de cinco segundos
  delay(5000);

  //Imprime con la operacion and
  Serial.println(num & num2);

  //100
  //101
  //=100 es 4 en decimal
}

void loop()
{

}
```

### El operador or "|"

```c++
void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  int num = 4; //100 en binario
  int num2 = 5; //101 en binario

  //Retardo de cinco segundos
  delay(5000);

  //Imprime con la operacion and
  Serial.println(num | num2);

  //100
  //101
  //=101 es 5 en decimal
}

void loop()
{

}
```

### Operador not "~"

```c++
//Binario de 32 bits
unsigned int x = 1; //00000000000000000000000000000001 en binario
unsigned int y = ~x; //11111111111111111111111111111110 esta negado

void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  //Retardo de cinco segundos
  delay(5000);

  //Imprime el resultado de 4.294.967.294
  Serial.println(y);
}

void loop() 
{

}
```

### Operador xor "^"
```c++
void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  int num = 4; //100 en binario
  int num2 = 5; //101 en binario

  //Retardo de cinco segundos
  delay(5000);

  //Imprime con la operacion and
  Serial.println(num ^ num2);

  //100
  //101
  //=001 es 1 en decimal
}

void loop()
{

}
```

### Operador de desplazamiento hacia la izquierda "<<"
* Los numeros enteros se almacenan en la memoria como una conjunto de bits
* El numero 6 decimal en binario de 32 bits es: ``` 00000000 00000000 00000000 00000110 ```
* Al hacer el desplazamiento ( 6 << 1) entregara como resultado el numero 12: ``` 00000000 00000000 00000000 00001100 ```


```c++
//Binario de 32 bits
int num = 6; //00000000000000000000000000000110 en binario
int num2 = 1;//00000000000000000000000000000001 en binario

void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  //Retardo de cinco segundos
  delay(5000);

  //Hace el desplazamiento a la izquierda y muestra el resultado de 12
  Serial.println(num << num2);

}

void loop()
{

}
```

### Operador de desplazamiento hacia la derecha ">>"
El desplazamiento aritmetico a la derecha es exactamente igual que el desplazamiento logico a la derecha, excepto que en lugar de rellenar con cero, rellena con el bit mas significativo, esto se debe a que el bit mas significativo es el bit de signo , o el bit que distingue los números positivos y negativos. Al rellenar con el bit más significativo, el desplazamiento aritmético a la derecha conserva el signo.

* Los numeros enteros se almacenan en la memoria como una conjunto de bits
* El numero 12 decimal en binario de 32 bits es: ``` 00000000 00000000 00000000 00001100 ```
* Al hacer el desplazamiento ( 12 << 1) entregara como resultado el numero 6: ``` 00000000 00000000 00000000 00000110 ```

```c++
//Binario de 32 bits
int num = 12; //00000000000000000000000000001100 en binario
int num2 = 1;//00000000000000000000000000000001 en binario

void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  //Retardo de cinco segundos
  delay(5000);

  //Hace el desplazamiento a la derecha y muestra el resultado de 6
  Serial.println(num >> num2);

}

void loop()
{

}
```
