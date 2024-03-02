# Cálculo de Probabilidade com Teorema de Bayes em Python

Este é um exemplo simples de como calcular a probabilidade de uma peça defeituosa ter sido produzida por uma máquina específica, usando o Teorema de Bayes.

## Requisitos

Certifique-se de ter o Python instalado em sua máquina.

## Execução

1. Clone o repositório:

    ```bash
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd nome-do-repositorio
    ```

3. Execute o script Python:

    ```bash
    python bayes_calculations.py
    ```

O script realizará os cálculos e imprimirá a probabilidade de uma peça defeituosa ter sido produzida pela Máquina A.

## Explicação

O cálculo da probabilidade é feito utilizando o Teorema de Bayes. Abaixo está o código Python explicado passo a passo.

```python
# bayes_calculations.py

# Probabilidades fornecidas no enunciado
P_A = 0.60  # Probabilidade de a peça ser da Máquina A
P_B = 0.40  # Probabilidade de a peça ser da Máquina B
P_D_A = 0.05  # Probabilidade de a peça ser defeituosa dado que foi produzida pela Máquina A
P_D_B = 0.08  # Probabilidade de a peça ser defeituosa dado que foi produzida pela Máquina B

# Calculando P(D), a probabilidade de uma peça ser defeituosa
P_D = P_D_A * P_A + P_D_B * P_B

# Calculando P(A|D), a probabilidade de a peça ser da Máquina A dado que é defeituosa
P_A_D = (P_D_A * P_A) / P_D

# Imprimindo o resultado
print(f"A probabilidade de uma peça defeituosa ser da Máquina A é aproximadamente: {P_A_D * 100:.2f}%")

# Cálculo de Probabilidade com Teorema de Bayes em Python para Máquina B

# Probabilidades fornecidas no enunciado
P_A = 0.60  # Probabilidade de a peça ser da Máquina A
P_B = 0.40  # Probabilidade de a peça ser da Máquina B
P_D_A = 0.05  # Probabilidade de a peça ser defeituosa dado que foi produzida pela Máquina A
P_D_B = 0.08  # Probabilidade de a peça ser defeituosa dado que foi produzida pela Máquina B

# Calculando P(D), a probabilidade de uma peça ser defeituosa
P_D = P_D_A * P_A + P_D_B * P_B

# Calculando P(B|D), a probabilidade de a peça ser da Máquina B dado que é defeituosa
P_B_D = (P_D_B * P_B) / P_D

# Imprimindo o resultado
print(f"A probabilidade de uma peça defeituosa ser da Máquina B é aproximadamente: {P_B_D * 100:.2f}%")

