lista 2
### Exercicio 1
### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite o primeiro número}}
B --> C[\num1\]
C --> D{{Digite o segundo número}}
D --> E[\num2\]
E --> F{{Digite o terceiro número}}
F --> G[\num3\]
G --> H{{Digite o quarto número}}
H --> I[\num4\]
I --> J[soma = num1 + num2 + num3 + num4]
J --> K[media = soma / 4]
K --> L{{'A média é: ', media}}
L --> M([FIM])
```
### Pseudocodigo
```
1  ALGORITMO calcular_media
2  DECLARE num1, num2, num3, num4, soma, media: REAL
3  INICIO
4    ESCREVA "Digite o primeiro número: "
5    LEIA num1
6    ESCREVA "Digite o segundo número: "
7    LEIA num2
8    ESCREVA "Digite o terceiro número: "
9    LEIA num3
10   ESCREVA "Digite o quarto número: "
11   LEIA num4
12   soma = num1 + num2 + num3 + num4
13   media = soma / 4
14   ESCREVA "A média é: ", media
15 FIM

```
### Teste de mesa


| Teste | num1 | num2 | num3 | num4 | soma (cálculo esperado) | média (cálculo esperado) | Saída esperada |
| ----- | ---- | ---- | ---- | ---- | ----------------------- | ------------------------ | --------------- |
| 1     | 2    | 4    | 6    | 8    | 20 (2 + 4 + 6 + 8)      | 5                        | "A média é: 5"  |

### Exercicio 2
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite a temperatura em Celsius C}}
B --> C[\temp_C\]
C --> D[Converter para Fahrenheit]
D --> E[temp_F = 9/5 * temp_C + 32]
E --> F{{A temperatura em Fahrenheit é: , temp_F}}
F --> G([FIM])
```
### Pseucodigo
```
1  ALGORITMO converter_temperatura
2  DECLARE temp_C, temp_F: REAL
3  INICIO
4    ESCREVA "Digite a temperatura em Celsius (C): "
5    LEIA temp_C
6    temp_F = (9/5) * temp_C + 32
7    ESCREVA "A temperatura em Fahrenheit é: ", temp_F
8  FIM

```
### Teste de mesa
| Teste | temp_C | temp_F (cálculo esperado) | Saída esperada |
| ----- | ------ | -------------------------- | --------------- |
| 1     | 0      | 32                         | "A temperatura em Fahrenheit é: 32" |

### Exercicio 3

### Fluxograma
```mermaid
flowchart TD
A([INÍCIO]) --> B{{Digite o primeiro número}}
B --> C[\num1\]
C --> D{{Digite o segundo número}}
D --> E[\num2\]
E --> F{{Digite o operador +, -, *, /}}
F --> G[\operador\]
G --> H{operador é '+'}
H -- SIM --> I{Efetuar adição}
I --> J[resultado = num1 + num2]
J --> K{{'O resultado da adição é: ', resultado}}
K --> L([FIM])
H -- NÃO --> M{operador é '-'}
M -- SIM --> N{Efetuar subtração}
N --> O[resultado = num1 - num2]
O --> K
M -- NÃO --> P{operador é '*'}
P -- SIM --> Q{Efetuar multiplicação}
Q --> R[resultado = num1 * num2]
R --> K
P -- NÃO --> S{operador é '/'}
S -- SIM --> T{Verificar divisão por zero}
T -- SIM --> U[Se num2 != 0 então calcular divisão]
U --> V[resultado = num1 / num2]
V --> K
T -- NÃO --> W[Escrever Erro: Divisão por zero.]
W --> L
S -- NÃO --> X[Escrever Operador inválido.]
X --> L
```
### Pseudocodigo
```
1  ALGORITMO calculadora
2  DECLARE num1, num2, resultado: REAL
3  DECLARE operador: CARACTERE
4  INICIO
5    ESCREVA "Digite o primeiro número: "
6    LEIA num1
7    ESCREVA "Digite o segundo número: "
8    LEIA num2
9    ESCREVA "Digite o operador (+, -, *, /): "
10   LEIA operador
11   SE operador = '+' ENTAO
12     resultado = num1 + num2
13     ESCREVA "O resultado da adição é: ", resultado
14   SENAO SE operador = '-' ENTAO
15     resultado = num1 - num2
16     ESCREVA "O resultado da subtração é: ", resultado
17   SENAO SE operador = '*' ENTAO
18     resultado = num1 * num2
19     ESCREVA "O resultado da multiplicação é: ", resultado
20   SENAO SE operador = '/' ENTAO
21     SE num2 != 0 ENTAO
22       resultado = num1 / num2
23       ESCREVA "O resultado da divisão é: ", resultado
24     SENAO
25       ESCREVA "Erro: Divisão por zero."
26     FIM_SE
27   SENAO
28     ESCREVA "Operador inválido."
29   FIM_SE
30 FIM

```
