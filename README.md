# Operador de Nivel de Bits

### El operador and "&" 

```c++
void setup() 
{
Serial.begin(115200);

int num = 4;
int num2 = 5;

delay(5000);

Serial.println(num & num2);
}

void loop() {

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

### Operador not "~" aun no entiendo como funciona

```c++
void setup() 
{
Serial.begin(115200);

int num = 4;
int num2 = 5;

delay(5000);

//0000000000000101
//1111111111111010

//con signo
Serial.println(~5);

//sin signo
Serial.println(~(unsigned int)5);
}

void loop() {

}
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

