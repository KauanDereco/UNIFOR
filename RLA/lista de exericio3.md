### Exercicio 1
```mermaid
flowchart TD
A([INÍCIO]) --> B{{Digite um número inteiro positivo}}
B --> C[\numero\]
C --> D{Verificar se número é negativo}
D -- SIM --> E{{Exibir mensagem de erro e solicitar novo número}}
E --> F[ESCREVA Número inválido. Por favor, digite um número inteiro positivo.]
F --> B
D -- NÃO --> G{{Verificar se número é par ou ímpar}}
G --> H{numero MOD 2 = 0}
H -- SIM --> I{{Exibir Número é par}}
I --> J[ESCREVA numero, é um número par.]
J --> K([FIM])
H -- NÃO --> L{{Exibir Número é ímpar}}
L --> M[ESCREVA numero,  é um número ímpar.]
M --> K

```
### Pseudocodigo
```
1  ALGORITMO verificar_par_ou_impar
2  DECLARE numero: INTEIRO
3  INICIO
4    REPITA
5        ESCREVA "Digite um número inteiro positivo: "
6        LEIA numero
7        
8        SE numero < 0 ENTÃO
9            ESCREVA "Número inválido. Por favor, digite um número inteiro positivo."
10       FIM_SE
11   ATÉ que numero >= 0
12   
13   SE numero MOD 2 = 0 ENTÃO
14       ESCREVA numero, " é um número par."
15   SENÃO
16       ESCREVA numero, " é um número ímpar."
17   FIM_SE
18   
19   FIM
```
### Teste de mesa
Vamos criar uma tabela semelhante usando o pseudocódigo fornecido:

| número | número >= 0 | resto | resto == 0 | Saída |
| ------ | ----------- | ----- | ---------- | ------|
| -1     | F           |       |            | "Número inválido. Por favor, digite um número inteiro positivo." |
| 0      | V           | 0     | V          | "0 é um número par." |
| 13     | V           | 1     | F          | "13 é um número ímpar." |
| 30     | V           | 0     | V          | "30 é um número par." |

