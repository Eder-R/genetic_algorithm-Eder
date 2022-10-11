# Genetic_Algorithm

## Introdução

Você ficará isolado na natureza selvagem. A única coisa que você poderá levar é uma mochila que suporta no máximo 30 kg. Você possui diversos itens de sobrevivência, cada um possui "pontos de sobrevivência" (dados para cada item de acordo com a tabela).

## Objetivo

---

Faça um fork do projeto em: <https://github.com/gregori/genetic_algorithm> e baseie-se nele.

Seu objetivo é maximizar os pontos de sobrevivência.

| Item          | Peso  | Pontos|
|---------------|-------|-------|
|Saco de dormir |  15   |   15  |
|Corda          |  03   |   10  |
|Canivete       |  02   |   10  |
|Tocha          |  05   |   05  |
|Garrafa        |  09   |   08  |
|Comida         |  20   |   17  |

---

## Dicas

---

### 1: Você basicamente precisará alterar a função cal_pop_fitness - aqui você deverá calcular a soma dos pontos de cada cromossomo. E eliminar as pontuações cujos pesos sejam MAIORES que 30kg (para isso, você pode fazer com que a pontuação seja um número negativo bem pequeno, como -9999999, nesses casos)

---

### 2: Você também precisará alterar a função mutation. A diferença aqui é que você não deve somar um valor aleatório. Simplesmente faça abs(valor_atual - 1), na hora de calcular a variação

---

### 3: Lembre-se que você vai ter que gerar um conjunto populacional em que os valores dos genes são 0 ou 1 (item ausente ou presente na mochila). Para isso você também precisa alterar a forma de gerar a população inicial, no main.py (dica, veja o método randint da biblioteca numpy)

---

### 4: Experimente aumentar o número de gerações e mexer no número de soluções por população (por exemplo 100 gerações, 10 soluções por população). Veja quantas gerações você precisa para obter o valor máximo de pontos
