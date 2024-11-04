# Atividade 02

### Aluno: João Pedro Martins Andrade

### 01. Escreva uma função que receba uma lista de números e retorne outra lista com os números ímpares.
```python
def filtrar_impares(lista):
    return [num for num in lista if num % 2 != 0]
```

### 02. Escreva uma função que receba uma lista de números e retorne outra lista com os números primos presentes.
```python
def filtrar_primos(lista):
    def eh_primo(n):
        if n < 2:
            return False
        for i in range(2, int(n ** 0.5) + 1):
            if n % i == 0:
                return False
        return True
    return [num for num in lista if eh_primo(num)]
```

### 03. Escreva uma função que receba duas listas e retorne outra lista com os elementos que estão presentes em apenas uma das listas.
```python
def diferenca_simetrica(lista1, lista2):
    return list(set(lista1).symmetric_difference(lista2))
```

### 04. Dada uma lista de números inteiros, escreva uma função para encontrar o segundo maior valor na lista.
```python
def segundo_maior(lista):
    lista_unica = list(set(lista))  # Remove duplicados
    lista_unica.sort(reverse=True)  # Ordena em ordem decrescente
    return lista_unica[1] if len(lista_unica) > 1 else None
```

### 05. Crie uma função que receba uma lista de tuplas, cada uma contendo o nome e a idade de uma pessoa, e retorne a lista ordenada pelo nome das pessoas em ordem alfabética.
```python
def ordenar_por_nome(lista_tuplas):
    return sorted(lista_tuplas, key=lambda pessoa: pessoa[0])
```

### 06. Observe os espaços sublinhados e complete o código.
```matplotlib```;<br>
```np```;<br>
```row```;<br>
```col```;<br>
```fontsize```;<br>
```4```.

### 07. Observe os espaços sublinhados e complete o código.
```matplotlib```;<br>
```matplotlib.pyplot```;<br>
```linspace```;<br>
```sin```;<br>
```fig, ax```;<br>
```plot(x, y)```.

### 08. Utilizando pandas, como realizar a leitura de um arquivo CSV em um DataFrame e exibir as primeiras linhas?
Para realizar essa leitura precisa utilizar ```pd.read_csv('caminho/do/arquivo.csv')``` para lê o arquivo e depois guardar em uma variável chamada ```df```. Depois executa ```print(df.head())``` para apresentar as primeiras linhas.

### 09. Utilizando pandas, como selecionar uma coluna específica e filtrar linhas em um “DataFrame” com base em uma condição?
Para selecionar uma coluna específica e filtrar linhas em um ```DataFrame``` com pandas, primeiro importe a biblioteca usando ```import pandas as pd```. Crie seu ```DataFrame com df = pd.DataFrame(dados)```. Para filtrar, use ```resultado = df.loc[df['Idade'] > 30, 'Nome']``` e, em seguida, imprima o resultado com ```print(resultado)```.

### 10. Utilizando pandas, como lidar com valores ausentes (NaN) em um DataFrame?
Para lidar com valores ausentes (NaN) em um ```DataFrame``` com pandas, primeiro importe a biblioteca usando ```import pandas as pd```. Carregue seu ```DataFrame``` com ```df = pd.read_csv('caminho/do/arquivo.csv')```. Para verificar valores ausentes, use ```print(df.isnull().sum())```. Para remover linhas com NaN, utilize ```df = df.dropna()```. Se preferir preencher os valores ausentes, use ```df = df.fillna(valor)```, onde ```valor``` pode ser um número ou uma string.