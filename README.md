# 👩‍🔬🎲Estatística para Ciência de Dados.

### Minhas anotações sobre Amostragem.

---

Sumário

* População e Amostra
* Técnicas de amostragem
* Amostragem aleatória simples e sistemática
* Amostragem estratificada e por conglomerados
* Calculando amostras

---

### Conceitos

* Uma população é o conjunto de dados que contém todas as observações possíveis, contendo todo e qualquer grupo que possa existir para esses dados.

Como considera todas as observações existentes, qualquer análise feita utilizando a população reflete a realidade e não possui qualquer erro intrínseco; chamamos as medidas que calculamos utilizando a população de parâmetros.

* Uma amostra é um subconjunto da população, é a parte do todo que é usada para representar a população.

Como considera apenas parte das observações existentes, qualquer análise feita utilizando uma amostra possui uma margem de erro intrínseca; chamamos as medidas que calculamos utilizando a população de estimativas.

E uma boa amostra significa que seus resultados estão mais próximos da realidade.

* Amostragem é o processo de seleção de observações da população que irão compor uma amostra.

---

### Temos várias técnicas para amostrar dados, mas 4 se destacam como as mais úteis e populares:

* Amostragem aleatória simples: Selecionamos de forma aleatória as observações que irão compor a amostra. Esse tipo de amostragem é a mais utilizada e popular.

Vantagens: Evita o erro sistemático e viés de seleção. Tende a ser simples de se planejar e comunicar aos outros.

Desvantagens: Tende a ter uma execução complexa e cara. Eventualmente, pode não representar bem subgrupos populacionais.

* Amostragem sistemática: Selecionamos uma regra de seleção de observações para compor a amostra.

Vantagens: Mais rápida de se implementar do que a amostragem aleatória simples.

Desvantagens: Eventualmente, pode não representar bem subgrupos populacionais. A ordenação dos participantes pode ser igual a uma ordenação existente, mas desconhecida, na população.

* Amostragem aleatória estratificada: Selecionamos subgrupos heterogêneos entre si (mas as observações dentro dos subgrupos são homogêneas). 
 E fazemos uma amostragem aleatória simples para cada estrato, juntando os resultados para compor a amostra final.
 
 Vantagens: Evita sub-representação de grupos pouco frequentes.
 
 Desvantagens: É preciso conhecer os estratos e sua execução é cara e custosa.

* Amostragem aleatória por conglomerados: Selecionamos subgrupos homogêneos entre si (mas as observações dentro dos subgrupos são heterogêneas).

Vantagens: Quando a identificação dos elementos da população é difícil, os conglomerados aparecem como solução.
A população já está dividida naturalmente.

Desvantagens: Os extratos não serem homogêneos entre eles.

---

### Calculando amostras

* Jupyter é uma IDE (Integrated Development Environment ou Ambiente de Desenvolvimento Integrado) utilizado para analisar dados.

É open source e o nome vem de 3 linguagens de programação: Julia, Python e R.

---

* O Python tem seu método bult-in para cálculo de amostras aleatórias.

from random import sample
populacao = [1,2,3]
sample (populacao, 2)


---

* A biliotecca pandas é a mais utilizada em Python para análise de dados.

import pandas
df = pandas.DataFrame(populacao, columns = ["values"])
df.sample(n = 4)

values
0  1
1  2
2  3
3  4

Na primeira coluna ficam os indices.

---

Podemos também passar a proporção do todo que queremos na queremos na nossa amostra, ao invés de passar o tamanho da amostra que queremos.

populacao = [1,2,3,4,5,6,7,8,9,10,11,12]
df = pandas.DataFrame(populacao, columns = ["values"]
df.sample(frac = 0.33)

---

🔎 Kaggle é uma plataforma para aprendizado de ciência de dados.

É também uma comunidade, a maior da internet, para assuntos relacionados com Data Science.

🕮 Conceitos e análises estatísticas com R e JASP.



