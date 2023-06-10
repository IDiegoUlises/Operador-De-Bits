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
Serial.begin(115200);

int num = 4;
int num2 = 5;

delay(5000);

Serial.println(num | num2);
}

void loop() {

}
```

### Operador not "~"

```c++
unsigned int x = 1;
 unsigned int y= ~x;

void setup() {
Serial.begin(115200);
delay(5000);

Serial.println(y);
}

void loop() {
  // put your main code here, to run repeatedly:

}
//binario de 32 bits
//00000000000000000000000000000001 es 1 
//11111111111111111111111111111110 en decimal 4.294.967.294

```

### Operador xor "^"
```c++
void setup() 
{
Serial.begin(115200);

int num = 4;
int num2 = 5;

delay(5000);


Serial.println(12 ^ 10);

}

void loop() {

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
