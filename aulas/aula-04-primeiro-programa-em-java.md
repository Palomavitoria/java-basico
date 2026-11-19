# Aula 04 – Primeiro Programa em Java ☕

## 📚 Conteúdo da aula

- Comando de pacotes;
- Cabeçalho da classe;
- Chaves;
- Blocos de código;
- Método principal;
- `package`;
- `class`;
- `main`;
- Técnicas de nomeação e identificação;
- Diferença entre letras maiúsculas e minúsculas;
- Atalho `sout + Tab`;
- Camel Case;
- Regras de nomenclatura;
- Case Sensitive.

---

## 1. Estrutura de um programa Java

Todo programa Java possui uma estrutura organizada, formada por declarações, classes, métodos e blocos de código.

Para começar a programar, é importante compreender a função de cada elemento.

## 2. Comando de pacotes – `package`

O comando `package` é utilizado para definir o pacote ao qual uma classe pertence.

Os pacotes servem para organizar as classes de um projeto, facilitando sua identificação e manutenção.

Exemplo:

```java
package com.mycompany.primeiroprograma;
```

Nesse exemplo, a classe pertence ao pacote `com.mycompany.primeiroprograma`.

**Importante:** a declaração de `package`, quando utilizada, deve aparecer no início do arquivo Java, antes das declarações de importação.

## 3. Cabeçalho da classe – `class`

A palavra-chave `class` é utilizada para declarar uma classe em Java.

Uma classe funciona como uma estrutura que reúne atributos e métodos.

Exemplo:

```java
public class PrimeiroPrograma {

}
```

Nesse exemplo:

- `public`: modificador de acesso que permite que a classe seja acessada de outros pacotes.
- `class`: palavra-chave utilizada para declarar uma classe.
- `PrimeiroPrograma`: nome da classe.
- `{ }`: delimitam o corpo da classe.

**Convenção:** nomes de classes devem começar com letra maiúscula e utilizar Camel Case quando houver mais de uma palavra.

## 4. Chaves e blocos de código

As chaves `{ }` são utilizadas para delimitar blocos de código em Java.

Elas indicam onde começa e onde termina uma estrutura.

Exemplo:

```java
public class PrimeiroPrograma {

    public static void main(String[] args) {

        System.out.println("Olá, Mundo!");

    }

}
```

Nesse exemplo, temos:

- Um bloco que delimita a classe;
- Um bloco que delimita o método principal;
- Uma instrução dentro do método.

As chaves são fundamentais para organizar e estruturar o programa.

## 5. Método principal – `main`

O método `main` é o ponto de entrada de uma aplicação Java tradicional.

É a partir dele que a execução do programa começa.

Sua declaração mais comum é:

```java
public static void main(String[] args) {

}
```

Entendendo cada parte:

| Elemento | Significado |
|---|---|
| `public` | Permite que o método seja acessado externamente. |
| `static` | Permite executar o método sem criar um objeto da classe. |
| `void` | Indica que o método não retorna um valor. |
| `main` | Nome do método principal reconhecido pelo iniciador da aplicação Java. |
| `String[] args` | Recebe argumentos que podem ser passados ao programa pela linha de comando. |

## 6. Palavras e comandos importantes

### `package`

Define o pacote ao qual a classe pertence.

### `class`

Declara uma classe.

### `main`

É o método principal, utilizado como ponto de entrada de uma aplicação Java tradicional.

### `System.out.println()`

É utilizado para exibir informações no console e pular uma linha após a impressão.

Exemplo:

```java
System.out.println("Olá, Mundo!");
```

Resultado:

```text
Olá, Mundo!
```

### Atalho `sout + Tab`

No Apache NetBeans, o atalho `sout` seguido de `Tab` pode ser utilizado para completar automaticamente a instrução:

```java
System.out.println();
```

Isso facilita a escrita do código e economiza tempo durante o desenvolvimento.

---

## 7. Técnicas de nomeação e identificação

Na programação, é importante utilizar nomes que facilitem a identificação de classes, métodos, variáveis e outros elementos.

Java possui convenções de nomenclatura que ajudam a manter o código organizado e legível.

### Diferença entre letras maiúsculas e minúsculas

Java é uma linguagem **Case Sensitive**, ou seja, diferencia letras maiúsculas de letras minúsculas.

Exemplo:

```java
String nome = "Paloma";
String Nome = "Vitória";
```

Nesse caso, `nome` e `Nome` são identificadores diferentes.

Observe também:

- `class` é uma palavra-chave válida.
- `Class` não é a mesma palavra-chave.
- `main` e `Main` são nomes diferentes.

Por isso, é necessário prestar atenção às letras utilizadas na escrita dos códigos.

## 8. Camel Case

Camel Case é uma convenção de nomenclatura utilizada para formar nomes compostos por mais de uma palavra, sem utilizar espaços.

A primeira letra de cada palavra, a partir da segunda, é escrita em maiúscula.

Exemplo:

```text
primeiroPrograma
nomeCompleto
calcularMedia
dataNascimento
```

### Principais regras de nomenclatura em Java

**Classes: Pascal Case**

Os nomes das classes começam com letra maiúscula e cada palavra seguinte também começa com letra maiúscula.

Exemplos:

```java
PrimeiroPrograma
CadastroAluno
CalculadoraSimples
```

**Variáveis e métodos: Camel Case**

Começam com letra minúscula e utilizam letra maiúscula no início das palavras seguintes.

Exemplos:

```java
nomeCompleto
idadeAluno
calcularMedia()
mostrarResultado()
```

**Constantes: letras maiúsculas**

Por convenção, constantes são escritas com letras maiúsculas, separando palavras com `_`.

Exemplos:

```java
VALOR_MAXIMO
TAXA_JUROS
PI
```

**Pacotes: letras minúsculas**

Os nomes dos pacotes são escritos em letras minúsculas.

Exemplos:

```java
com.mycompany.primeiroprograma
br.com.projeto.calculadora
```

### Resumo das convenções

| Elemento | Convenção | Exemplo |
|---|---|---|
| Classes | Pascal Case | `PrimeiroPrograma` |
| Variáveis | Camel Case | `nomeCompleto` |
| Métodos | Camel Case | `calcularMedia()` |
| Constantes | Letras maiúsculas | `VALOR_MAXIMO` |
| Pacotes | Letras minúsculas | `com.projeto.java` |

**Observação:** essas são convenções de nomenclatura. Java também possui regras próprias sobre quais caracteres podem ser utilizados em identificadores.

---

## 9. Código desenvolvido durante a aula

Durante a aula, foi desenvolvido o primeiro programa em Java, responsável por exibir três mensagens no console.

### Código-fonte

```java
package com.mycompany.primeiroprograma;

import java.io.PrintStream;
import java.nio.charset.StandardCharsets;

public class PrimeiroPrograma {

    public static void main(String[] args) {

        System.setOut(new PrintStream(System.out, true, StandardCharsets.UTF_8));

        System.out.println("Olá, Mundo!");
        System.out.println("Programação é muito interessante!");
        System.out.println("Você está aprendendo Java!");
    }

}
```

### Explicação do código

**1. Declaração do pacote**

```java
package com.mycompany.primeiroprograma;
```

Define o pacote ao qual a classe pertence.

**2. Importações**

```java
import java.io.PrintStream;
import java.nio.charset.StandardCharsets;
```

Importa as classes necessárias para configurar a saída de texto utilizando UTF-8.

- `PrintStream`: permite trabalhar com fluxos de saída de dados.
- `StandardCharsets`: fornece conjuntos de caracteres padronizados, incluindo UTF-8.

**3. Declaração da classe**

```java
public class PrimeiroPrograma {
```

Declara a classe pública chamada `PrimeiroPrograma`.

**4. Método principal**

```java
public static void main(String[] args) {
```

Define o método principal, responsável por iniciar a execução do programa.

**5. Configuração da codificação UTF-8**

```java
System.setOut(new PrintStream(System.out, true, StandardCharsets.UTF_8));
```

Configura a saída padrão do programa para utilizar a codificação UTF-8.

Isso ajuda a exibir corretamente caracteres especiais, como acentos e cedilha, no console.

**6. Exibição das mensagens**

```java
System.out.println("Olá, Mundo!");
System.out.println("Programação é muito interessante!");
System.out.println("Você está aprendendo Java!");
```

Cada instrução `System.out.println()` exibe uma mensagem e pula para a próxima linha.

### Resultado da execução

```text
Olá, Mundo!
Programação é muito interessante!
Você está aprendendo Java!
```

---

## 📌 Resumo para revisão

- `package`: define o pacote ao qual a classe pertence.
- `class`: declara uma classe.
- `main`: método principal e ponto de entrada de uma aplicação Java tradicional.
- `{ }`: delimitam blocos de código.
- `System.out.println()`: exibe informações no console e pula uma linha.
- `sout + Tab`: atalho do NetBeans para completar `System.out.println()`.
- IDE: ambiente que reúne ferramentas para desenvolver programas.
- Camel Case: convenção de nomenclatura que utiliza letras maiúsculas para separar palavras.
- Pascal Case: convenção em que cada palavra começa com letra maiúscula.
- Case Sensitive: característica que faz Java diferenciar letras maiúsculas e minúsculas.
- UTF-8: codificação de caracteres que permite representar letras acentuadas e outros símbolos.

## 📌 Pontos principais para revisão

1. Todo programa Java é organizado em classes.
2. O comando `package` organiza as classes em pacotes.
3. A palavra-chave `class` declara uma classe.
4. O método `main` é o ponto de entrada de uma aplicação Java tradicional.
5. As chaves delimitam os blocos de código.
6. Java diferencia letras maiúsculas e minúsculas.
7. Classes utilizam Pascal Case por convenção.
8. Variáveis e métodos utilizam Camel Case por convenção.
9. Constantes são geralmente escritas em letras maiúsculas.
10. `System.out.println()` é utilizado para exibir mensagens no console.

## 🎯 Objetivo da aula

Compreender a estrutura básica de um programa Java, conhecer os principais comandos e elementos utilizados na criação de uma classe, entender o funcionamento do método principal e aprender as convenções de nomenclatura utilizadas na linguagem.
