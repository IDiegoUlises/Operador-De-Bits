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
```c++
void setup() 
{
Serial.begin(115200);

int num = 4;
int num2 = 5;

delay(5000);


Serial.println(4 << 1);

}

void loop() {

}
```

### Operador de desplazamiento hacia la derecha ">>"

```c++
void setup() 
{
Serial.begin(115200);

int num = 4;
int num2 = 5;

delay(5000);


Serial.println(4 >> 1);

}

void loop() {

}
```
