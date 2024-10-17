# Atividade 01

### Aluno: João Pedro Martins Andrade

### 1. Explique, com suas palavras, o que é Machine Learning?
Machine Learning, ou Aprendizado de Máquina, é uma subárea de Inteligência Artificial, onde sistemas se utilizam
de uma base de dados para aprenderem e/ou se aperfeiçoarem sozinhos. O Aprendizado de Máquina é realizado
través da construção de algoritmos e modelos estatísticos que dão permissão aos sistemas realizarem tarefas sem
instrução específica.

### 2. Explique o conceito de conjunto de treinamento, conjunto de validação e conjunto de teste em Machine Learning.
* **Conjunto de Treinamento:** esse é o conjunto que utilizamos para _treinar_ o modelo; o algoritmo de aprendizado é ajustado com base nesse conjunto de dados, procurando por padrões e/ou relações.
* **Conjunto de Validação:** quando queremos _ajusta_ o modelo, utilizamos o conjunto de validação; ele funciona verificando o desempenho do modelo durante o treinamento, ajudando a evitar a perda de generalização, um conceito chamado de _overfitting_.
* **Conjunto de Teste:** já quando se quer _avaliar o desempenho_ do modelo, utilizamos o conjunto de teste; depois de ter treinado e ajustado os modelos, esse conjunto de dados entraem cena medindo como o modelo se comporta em dados que ele nunca viu antes.

### 3. Explique como você lidaria com dados ausentes em um conjunto de dados de treinamento.
Eu tentaria seguir os seguintes passos para tentar solucionar essa defasagem:
* O primeiro passo, e mais óbvio, seria consultar o(s) responsável(is) pela base de dados e tentar ver se realmente não teria como resgatar os dados com ele;
* Não logrando êxito na primeira opção, tentaria ver como treinar o modelo com os dados que tenho em mãos e já criar uma forma de coletar novos dados a partir daquele momento, para que essa falta de dados fosse suprida.

### 4. O que é uma matriz de confusão e como ela é usada para avaliar o desempenho de um modelo preditivo?
Matriz de Confusão é o nome atribuído a uma tabela que resume o desempenho de um modelo de classificação, onde se é comparado os valores reais com as previsões feitas pelo modelo. Ela é organizada em _Verdeiros Positivos_, _Falsos Positivos_, _Verdadeiros Negativos_ e _Falos Negativos_.

### 5. Em quais áreas (tais como construção civil, agricultura, saúde, manufatura, entre outras) você acha mais interessante aplicar algoritmos de Machine Learning?
Finanças; acho que é uma área interessante, tenho uma leve inclinação por essa área, e acredito que seria muito legal implementar algoritmos que viessem a contribuir para uma empresa com foco em finanças.