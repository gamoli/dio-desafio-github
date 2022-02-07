# C#

O C# (C-Sharp) é uma linguagem de alto nível fortemente tipada

### Comandos

- ``Console.WriteLine()``: Exibe argumento na tela com quebra de linha ao fim. Saudoso printf;
  - Variáveis podem ser passadas dentro da string de saída através da escrita de seus nomes entre chaves;
- ``Console.ReadLine()``: Lê dado inserido na tela e armazena no argumento da função. Saudoso scanf;
- ``dispose()``: desaloca objeto não gerenciado da memória;
- ``ToUpper()``: coloca a string em caixa alta;

### Tipos de Funções

- ``public``: Método acessível fora da classe;
- ``protected``: Acessível pela classe e seus herdeiros;
- ``private``: Acessível somente dentro do código da classe;
- ``... virtual``: Permite que uma classe herdeira sobrescreva o método (override);
- ``... override``: Método de classe filha que sobrescreve o da *base* de mesmo nome;
- ``... static``: Método acessível apenas pela classe e não por uma instância;

### Bibliotecas

- ``System``:
  - Biblioteca padrão C#;
  - Contem funcionalidades relacionadas ao console
    - ``System.Console.WriteLine``
    - ``System.Console.ReadLine``
- ``System.IO``: Biblioteca para operações com diretórios, arquivos e caminhos;
  - ``Directory.CreateDirectory()``;
  - ``Directory.Delete()``;
  - ``Directory.GetFiles()``;
  - ``File.CreateTExt()``;
  - ``File.AppendText()``;
  - ``File.Move()``;
  - ``File.Copy()``;
- ``System.Collections.Generic``: Biblioteca para uso de listas;
  - Utilizada para o uso de streams;

### Variáveis

- Varáveis int tem valor zero quando declaradas. Para poder ter valor nulo (null) deve ser declarado como nullable;
- Na manipulação de dados não gerenciados - arquivos, bancos de dados, etc - o uso da instrução ``using()`` elimina a necessidade do uso do ``dispose()`` para desalocar o objeto da memória.

### Classes

- Classes podem ter várias herdeiras mas apenas uma _parent class_;
- Métodos ``public static`` das classes pertecem às classes em si, não às instâncias;
- Para que variáveis de entrada em um método tenham valor alterado pelas sua execução no escopo externo ao método, estas variáveis deve ser passadas por referência(``ref``);
- Classes abstratas (``abstract``) não podem ser instanciadas. Servem apenas de molde para as classes filhas;
  - Seus métodos ``abstract`` deve ser sobrepostos (``override``) pelas classes filhas;
- Classes seladas (``sealed``) não podem ter classes filhas;
  - Métodos selados não podem ser sobrepostos em classes filhas;
- A classe ``System.Object`` é a mãe de todas as classes! Isso significa que há alguns métodos que todas classes podem utilizar por terem sido herdados da classe _Eva_:
  - ``Equals(object)``: Determina se objeto atualé igual ao especificado;
  - ``Equals(object, object)``: Determina se as instâcias de obejtos especificados são consideradas iguais;
  - ``Finalize()``: Permite que objeto tente liberar recursos e executar operações de limpeza antes de ser recuperado pela coleta de lixo (garbage colector);
  - ``GetHashCode()``: Função de Hash padrão;
  - ``GetType()``: Obtém o ``Type`` da instância atual;
  - ``MemberwiseClone()``: Cria uma cópia superficial do Object atual;
  - ``ReferenceEquals(Object, Object)``: Determina se as instâncias especificadas são a mesma instância;
  - ``ToString()``: Retorna uma cadeia de caracter que representa o objeto atual;

### Struct

- As Classes são tipos de referência ao passo que os Structs são tipos de valor;
- Os Structs são aceitam herença;

### Enum

- Quando não lhe é passado um tipo explcitamente, o Enum é dado como um ``int``;
  - E quando seus nomes não recebem valores associados de forma explícita, estes recebem valores incrementais interios a partir do 1;

### Interface

- É um contrato que pode ser implementado por uma classe;
- Uma classe pode implementar múltiplas interfaces;
- Não pode ser instanciada;
- As classes que implementarem uma interface devem implementar todos os métodos declarados pela interface;
  - Caso a interface tenha alguma implementação padrão - e não apenas a assinatura - de algum método, então esse não precisa ser implementado pela classe contratante;

### Arquivo

- Classes estáticas que auxiliam na manipulação de arquivos:
  - File;
  - Directory;
  - Path;
- Caracter coringa para filtro de busca: "*"

# Links úteis

- [Download .NET](https://dotnet.microsoft.com/download)
- [Documentação .NET](https://docs.microsoft.com/pt-br/dotnet)
- [.NET Foundation](https://dotnetfoundation.org)