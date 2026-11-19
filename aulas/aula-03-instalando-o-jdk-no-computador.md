# Aula 03 – Instalando o JDK no seu Computador ☕

## 📚 Conteúdo da aula

- IDE (Integrated Development Environment);
- RAD (Rapid Application Development);
- Edições do Java;
- Instalação e configuração do JDK.

---

## 1. IDE – Integrated Development Environment

IDE significa **Integrated Development Environment**, ou Ambiente de Desenvolvimento Integrado.

É um software que reúne ferramentas necessárias para facilitar o desenvolvimento de programas.

Uma IDE permite escrever, editar, compilar, executar e depurar códigos em um único ambiente.

### Principais recursos de uma IDE

- **Editor de código:** permite escrever e editar programas.
- **Compilador:** possibilita transformar o código-fonte em código executável ou intermediário.
- **Depurador (Debugger):** ajuda a identificar e corrigir erros no código.
- **Gerenciamento de projetos:** organiza arquivos e recursos de uma aplicação.
- **Autocompletar:** sugere comandos e completa trechos de código.

### Exemplos de IDEs

- Apache NetBeans;
- IntelliJ IDEA;
- Eclipse;
- Visual Studio Code (editor de código que pode ser configurado com recursos de desenvolvimento).

**Importante:** uma IDE facilita o desenvolvimento, mas não substitui o JDK. Para desenvolver aplicações Java, é necessário possuir um JDK compatível e configurado.

## 2. RAD – Rapid Application Development

RAD significa **Rapid Application Development**, ou Desenvolvimento Rápido de Aplicações.

É uma abordagem de desenvolvimento de software que busca acelerar a criação de aplicações por meio de ferramentas, componentes reutilizáveis e prototipagem.

O objetivo é desenvolver sistemas de maneira mais rápida, permitindo testar ideias e realizar melhorias durante o processo.

### Características do RAD

- Desenvolvimento rápido de aplicações;
- Reutilização de componentes;
- Criação de protótipos;
- Participação frequente dos usuários;
- Testes e melhorias durante o desenvolvimento.

### Relação entre RAD e IDE

Uma IDE pode oferecer ferramentas que facilitam o desenvolvimento rápido de aplicações.

Por exemplo, algumas IDEs permitem criar interfaces gráficas por meio de componentes visuais, reduzindo a necessidade de escrever manualmente todo o código.

**Importante:** IDE e RAD não são a mesma coisa. IDE é um ambiente de desenvolvimento, enquanto RAD é uma abordagem de desenvolvimento de software.

## 3. Edições do Java

A plataforma Java possui diferentes edições, desenvolvidas para atender a necessidades específicas.

As principais são:

### 3.1 Java SE – Standard Edition

Java SE significa **Java Platform, Standard Edition**.

É a edição padrão do Java, utilizada para desenvolver aplicações gerais.

Oferece recursos fundamentais da linguagem, como:

- Variáveis e tipos de dados;
- Estruturas condicionais;
- Estruturas de repetição;
- Classes e objetos;
- Programação Orientada a Objetos;
- Coleções;
- Manipulação de arquivos;
- Bibliotecas padrão.

É a edição utilizada como base para aprender Java e desenvolver aplicações de propósito geral.

### 3.2 Java EE – Enterprise Edition

Java EE significa **Java Platform, Enterprise Edition**.

Foi desenvolvida para aplicações corporativas e sistemas de maior complexidade, principalmente aplicações empresariais e sistemas web.

Atualmente, sua evolução é conhecida como **Jakarta EE**.

É utilizada em aplicações que podem envolver:

- Sistemas empresariais;
- Aplicações web;
- Serviços e APIs;
- Integração entre sistemas;
- Aplicações distribuídas.

### 3.3 Java ME – Micro Edition

Java ME significa **Java Platform, Micro Edition**.

Foi desenvolvida para dispositivos com recursos limitados, especialmente dispositivos móveis e embarcados.

Historicamente, foi utilizada em celulares e outros equipamentos eletrônicos com capacidade de processamento e memória reduzidas.

### Comparação das edições

| Edição | Significado | Finalidade |
|---|---|---|
| Java SE | Standard Edition | Aplicações gerais e aprendizado da linguagem. |
| Java EE | Enterprise Edition | Aplicações corporativas e empresariais. Atualmente evoluiu para Jakarta EE. |
| Java ME | Micro Edition | Dispositivos móveis e embarcados com recursos limitados. |

## 4. Instalação do JDK

JDK significa **Java Development Kit** e corresponde ao kit de desenvolvimento Java.

Ele reúne ferramentas necessárias para desenvolver, compilar e executar aplicações Java.

Para programar em Java, precisamos instalar um JDK compatível com o sistema operacional.

### Etapas da instalação

1. Acessar o site oficial da Oracle ou de outra distribuição do OpenJDK.
2. Escolher a versão do JDK compatível com o sistema operacional.
3. Baixar o instalador.
4. Executar o arquivo baixado.
5. Seguir as instruções do instalador.
6. Concluir a instalação.

### Verificando a instalação

Após instalar o JDK, podemos verificar se ele está funcionando por meio do Prompt de Comando do Windows (CMD).

Para verificar a versão do Java, utilizamos:

```bash
java -version
```

Para verificar a versão do compilador Java, utilizamos:

```bash
javac -version
```

Se os comandos apresentarem as versões instaladas, significa que o Java e o compilador estão disponíveis no terminal.

### Minha instalação

Neste curso, foi instalado o **Oracle JDK 27.0.1.1 (64 bits)** no Windows.

As verificações realizadas apresentaram:

```text
javac 27.0.1.1
```

E:

```text
java version "27.0.1.1"
```

Portanto, o JDK foi instalado e os comandos `java` e `javac` estão funcionando corretamente.

---

## 📌 Resumo para revisão

| Conceito | Significado | Função |
|---|---|---|
| IDE | Integrated Development Environment | Ambiente que reúne ferramentas para desenvolver programas. |
| RAD | Rapid Application Development | Abordagem que busca acelerar o desenvolvimento de aplicações. |
| Java SE | Standard Edition | Desenvolvimento de aplicações gerais. |
| Java EE | Enterprise Edition | Desenvolvimento de aplicações corporativas. Atualmente evoluiu para Jakarta EE. |
| Java ME | Micro Edition | Desenvolvimento para dispositivos com recursos limitados. |
| JDK | Java Development Kit | Kit de ferramentas para desenvolver e executar aplicações Java. |

## 📌 Pontos principais para revisão

- IDE significa Ambiente de Desenvolvimento Integrado.
- Uma IDE reúne ferramentas para escrever, executar, testar e depurar programas.
- RAD significa Desenvolvimento Rápido de Aplicações.
- RAD é uma abordagem de desenvolvimento, não uma linguagem de programação.
- Java SE é a edição padrão utilizada para aplicações gerais.
- Java EE foi direcionada ao desenvolvimento de aplicações empresariais e evoluiu para Jakarta EE.
- Java ME foi desenvolvida para dispositivos com recursos limitados.
- JDK é necessário para desenvolver aplicações Java.
- Os comandos `java -version` e `javac -version` permitem verificar a instalação do Java e do compilador.

## 🎯 Objetivo da aula

Compreender o conceito de IDE e RAD, conhecer as principais edições da plataforma Java e entender a importância da instalação do JDK para desenvolver e executar aplicações Java.
