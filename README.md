# Projeto: Calculadora Simples em Python

Este repositório contém um script Python simples que funciona como uma calculadora interativa de dois números, implementando as quatro operações básicas.

## Como Executar o Arquivo .sh

O arquivo `executar.sh` é um script de *shell* que facilita a execução do programa `calculadora.py`.

**Pré-requisitos:**

* **Python 3** instalado no sistema.
* **Sistema Operacional** baseado em Unix/Linux (ou um ambiente como o WSL no Windows).

**Passos para execução:**

1.  **Baixe/Clone** este repositório para o seu computador.
2.  Abra o **Terminal** ou **Prompt de Comando** na pasta do projeto.
3.  **Conceda permissão** de execução ao script:
    ```bash
    chmod +x executar.sh
    ```
4.  **Execute o script** `executar.sh`:
    ```bash
    ./executar.sh
    ```
5.  O programa solicitará seu nome, os dois números e a operação desejada (`+, -, *, /`).

## Explicação do Código em Python (`calculadora.py`)

O arquivo `calculadora.py` implementa uma calculadora simples com base em entradas do usuário.

### Funcionalidade

1.  **Entrada de Dados:** O script solicita o nome do usuário, dois números inteiros (`num1`, `num2`) e a operação a ser realizada (`+`, `-`, `*`, `/`).
2.  **Funções Dedicadas:** Quatro funções (`somar`, `subtrair`, `multiplicar`, `dividir`) são definidas para isolar e realizar cada operação matemática.
3.  **Lógica Condicional:** Uma estrutura de controle **`if/elif`** verifica qual operação o usuário digitou e chama a função correspondente, armazenando o resultado na variável `resultado`.
4.  **Saída de Dados:** O resultado final da operação é exibido na tela.

### Estrutura do Código

```python
# Coleta o nome e os números de entrada do usuário
nome = input('Olá como você se chama? ')
# ...
num1 = int(input('Digite um numero: '))
num2 = int(input('Digite outro numero: '))

# Definição das funções de operação
def somar(num1, num2):
    return num1 + num2
# ... (funções subtrair, multiplicar e dividir)

# Lógica de execução
operacao = input('Agora informa qual operação deseja realizar. (+, -, *, /): ')

if operacao == "+":
  resultado = somar(num1, num2)
# ... (outras condições elif)
