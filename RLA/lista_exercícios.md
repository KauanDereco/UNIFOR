
# UNIFOR

**Nome**: Nome do estudante
**Disciplina**: Raciocínio Lógico Algorítmico

## Lista 1 Exercício 1
### Fluxograma
```mermaid
flowchart TD
A([INÍCIO]) --> B{{Digite um número}}
B --> C[\número\]
C --> D{número > 0}
D --NÃO--> E[O número não é positivo!]
D --SIM--> F[resto = número % 2]
E --> Z([FIM])
F --> G{resto == 0}
G --NÃO--> H{{o número é ímpar!}}
G --SIM--> I{{o número é par!}}
H --> Z
I --> Z
```

### Pseudocódigo
```
1  ALGORÍTIMO verificapar_ímpar
2  DECLARE número, resto NUMÉRICO
3  ESCREVA "Digite um número: "
4  LEIA número
5  SE número > 0 ENTÃO
6    resto = número % 2
7    SE resto == 0 ENTÂO
8      ESCREVA "0 número é par!"
9    SENÃO
10     ESCREVA "O número é ímpar!"
11 SENÃO
12  ESCREVA "O número não positivo!"
13 FIM_ALGORITMO
```
#### Teste de mesa
| numero | numero >= 0 | resto | resto == 0 | Saída |
| -- | -- | -- | -- | -- | 
| -1 | F |   |   | "O número deve ser postivo!" |
| 0  | V | 0 | V | "O número é par!" |
| 13 | V | 1 | F | "O número é impar!" |
| 30 | V | 0 | V | "O número é par!" |

### EXERCICIO 2
```mermaid
graph TD;
    A[Início] --> B[Digite o salário atual];
    B --> C{Salário <= R$ 500?};
    C -->|Sim| D[NovoSalario = Salario * 1.2];
    C -->|Não| E[NovoSalario = Salario * 1.1];
    D --> F[Imprimir NovoSalario];
    E --> F;
    F --> G[Fim];

```
###PSEUDOCODIGO
```
1. Início
2. Digite o salário atual
3. Se salário <= R$ 500 então
4.     NovoSalario = Salario * 1.2 (aumento de 20%)
5. Senão
6.     NovoSalario = Salario * 1.1 (aumento de 10%)
7. Fim Se
8. Imprimir NovoSalario
9. Fim
```
Aqui está o teste de mesa para o fluxograma fornecido:

#### Teste de mesa
| Salário | Salário <= R$ 500? | NovoSalario | Saída |
| ------- | ------------------- | ----------- | ----- |
| R$ 300  | Sim                 | R$ 360      | R$ 360 impresso |
| R$ 600  | Não                 | R$ 660      | R$ 660 impresso |



