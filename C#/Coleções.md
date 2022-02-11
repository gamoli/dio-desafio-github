# Coleções

As coleções são tipos de dados vetorizados como arrays, matrizes, listas, filas, entre outros.

## Arrays

- Tem tipo e tamanho fixo em sua declaração;
- No C# há a classe Array - da biblioteca ``System`` - que já tem diversos métodos de manipulação de arrays implementados, como:
  - ``Array.Sort()``;
  - ``Array.Copy()``;
  - ``Array.Exists()``;
  - ``Array.TrueForAll()``;
  - ``Array.Find()``;
  - ``Array.IndexOf()``;
  - ``Array.Resize()``;
  - ``Array.ConvertAll()``;

## Coleções genéricas

No C#, através da biblioteca ``System.Collections.Generic``, é possível acessar as classes de coleções seguintes:
- ``Dictionary``: Coleções de pares chave-valor;
- ``List``: Lista de objetos que podem ser acessados por índice;
- ``Queue``: Coleção de objetos PEPS (FIFO) - Fila;
- ``SortedList``: Coleção de pares chave-valor classificadas por chavecom base numa implementação associada;
- ``Stack``: Coleção de objetos UEPS (LIFO) - Pilha;

Coleções genéricas possuem tipagem forte mas não requerem definição de tamanho fixo em sua declaração.

### Queue (Fila)

#### Comandos:
- ``.Enqueue()``: Adiciona item no final da fila;
- ``.Dequeue()``: Remove e retorna primeiro item da fila;
- ``.Peak()``: Retorna primeiro item da fila;

### Stack (Pilha)

#### Comandos:
- ``.Push()``: Adiciona item no topo da pilha;
- ``.Pop()``: Remove e retorna o item no topo da pilha;
- ``.Peak()``: Retorna o item do topo da pilha;

### Dictionary (Dicionário)

- A chave da coleção deve ser única;
- A chave é armazenada em hash;

#### Comandos:
- ``.Add()``: Adiciona item ao dicionário;
- ``<dicionário>[<chave>]``: Retorna a valor associado à chave;
- ``.Remove()``: Remove item do dicionário;
- ``.TryGetValue()``: Retorna valor lógico verdadeiro se encontra chave especificada e outa o valor do item. Do contrário, retorna valor lógico falso;

## LINQ - Language-Integrated Query

- Forma de de utilizar sintaxe padronizada de consulta para coleções de objetos;
- Biblioteca: ``System.Linq``;
- Pode-se usar de duas formas:
  - Formato Querry:  
    - > ``var querry =``  
      > ``from num in array``  
      > ``where num % 2 == 0``  
      > ``orderby num``  
      > ``select num;``
  - Formato Método:
    - > ``var querry = array.Where(num => num % 2 == 0).OrderBy(num => num).ToList();``

### Comandos:

- ``.Min()``: retorna o menor valor da coleção;
- ``.Max()``: retorna o maior valor da coleção;
- ``.Average()``: retorna o valor médio da coleção;
- ``.Sum()``: retorna a soma de todos os valores da coleção;
- ``.Distinct()``: retorna uma coleção sem elementos repetidos;