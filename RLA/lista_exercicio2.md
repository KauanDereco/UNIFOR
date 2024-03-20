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

