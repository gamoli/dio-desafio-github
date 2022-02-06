# C#

O C# (C-Sharp) é uma linguagem de alto nível fortemente tipada

### Comandos

- ``Console.WriteLine()``: Exibe argumento na tela com quebra de linha ao fim. Saudoso printf;
  - Variáveis podem ser passadas dentro da string de saída através da escrita de seus nomes entre chaves;
- ``Console.ReadLine()``: Lê dado inserido na tela e armazena no argumento da função. Saudoso scanf;
- ``dispose()``: desaloca objeto não gerenciado da memória;

### Tipos de Funções

- ``public``: Método acessível fora da classe;
- ``protected``: Acessível pela classe e seus herdeiros;
- ``private``: Acessível somente dentro do código da classe;
- ``... virtual``: Permite que uma classe herdeira sobrescreva o método (override);
- ``... override``: Método de classe filha que sobrescreve o da *base* de mesmo nome;
- ``... static``: Método acessível apenas pela classe e não por uma instância;

### Bibliotecas

- ``system``:
  - Biblioteca padrão C#;
  - Contem funcionalidades relacionadas ao console
    - ``System.Console.WriteLine``
    - ``System.Console.ReadLine``

### Comentários importantes

#### Variáveis

- Varáveis int tem valor zero quando declaradas. Para poder ter valor nulo (null) deve ser declarado como nullable;
- Na manipulação de dados não gerenciados - arquivos, bancos de dados, etc - o uso da instrução ``using()`` elimina a necessidade do uso do ``dispose()`` para desalocar o objeto da memória.

#### Classes

- Métodos ``public static`` das classes pertecem às classes em si, não às instâncias;
- Para que variáveis de entrada em um método tenham valor alterado pelas sua execução no escopo externo ao método, estas variáveis deve ser passadas como por referência(``ref``);