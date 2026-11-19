# Aula 02 – Como Funciona o Java ☕

## 📚 Conteúdo da aula

- Diferença entre JDK e JRE;
- O que é JDK e o que contém;
- O que é JRE e o que contém;
- Como funciona o ambiente Java;
- WORA (Write Once, Run Anywhere);
- JAVAC;
- JVM (Java Virtual Machine).

---

## 1. Como funciona o Java?

Java é uma linguagem de programação que possui um ambiente próprio para desenvolver e executar aplicações.

Para compreender seu funcionamento, é necessário conhecer três componentes fundamentais:

- **JDK:** kit de desenvolvimento Java.
- **JRE:** ambiente de execução Java.
- **JVM:** máquina virtual Java.

Cada um possui uma função específica dentro do funcionamento da plataforma Java.

## 2. JDK – Java Development Kit

JDK significa **Java Development Kit**, ou Kit de Desenvolvimento Java.

É o conjunto de ferramentas necessário para desenvolver programas em Java.

O JDK é utilizado principalmente por programadores, pois permite escrever, compilar, testar e executar aplicações.

### O que encontramos dentro do JDK?

Entre seus principais componentes estão:

- **JRE:** ambiente necessário para executar aplicações Java.
- **JAVAC:** compilador responsável por transformar o código-fonte Java em bytecode.
- **JVM:** máquina virtual responsável por executar o bytecode.
- **Ferramentas de desenvolvimento:** utilitários para compilar, executar, documentar e diagnosticar aplicações Java.

**Importante:** nas versões modernas do Java, a estrutura do JDK mudou. Desde o JDK 11, não existe mais uma instalação separada do JRE incluída como antigamente. O JDK contém os componentes necessários para desenvolver e executar aplicações, incluindo a JVM.

## 3. JRE – Java Runtime Environment

JRE significa **Java Runtime Environment**, ou Ambiente de Execução Java.

É o ambiente responsável por fornecer os componentes necessários para executar aplicações Java.

Diferentemente do JDK, o JRE não é destinado ao desenvolvimento de programas.

### O que encontramos dentro do JRE?

Tradicionalmente, o JRE possui:

- **JVM:** responsável por executar o bytecode.
- **Bibliotecas Java:** conjuntos de classes e recursos utilizados pelas aplicações.
- **Arquivos de suporte:** componentes necessários para o funcionamento do ambiente de execução.

**Importante:** nas versões antigas, o JRE era distribuído separadamente. Nas versões modernas, como o Java 27, não existe mais um JRE independente fornecido pela Oracle como nas versões anteriores.

## 4. Diferença entre JDK e JRE

A principal diferença está na finalidade de cada um.

| JDK | JRE |
|---|---|
| Kit de desenvolvimento Java. | Ambiente de execução Java. |
| Utilizado para desenvolver aplicações. | Utilizado para executar aplicações. |
| Possui ferramentas como o compilador JAVAC. | Não possui o conjunto completo de ferramentas de desenvolvimento. |
| Inclui os componentes necessários para executar aplicações. | Fornece os componentes necessários para a execução. |

### Resumindo:

- **JDK:** permite desenvolver e executar programas Java.
- **JRE:** fornece o ambiente necessário para executar programas Java.

## 5. WORA – Write Once, Run Anywhere

WORA significa **Write Once, Run Anywhere**, que em português significa:

**Escreva uma vez, execute em qualquer lugar.**

Esse conceito representa uma das principais características do Java: a portabilidade.

Isso significa que um programa Java pode ser desenvolvido em um sistema operacional e executado em outro, desde que exista um ambiente compatível com Java.

Exemplo:

Um programa desenvolvido no Windows pode ser executado no Linux ou macOS sem precisar ser reescrito especificamente para cada sistema.

Isso é possível porque o Java utiliza o bytecode e a JVM.

Cada sistema operacional possui uma implementação compatível da JVM, responsável por executar o mesmo bytecode naquele ambiente.

## 6. JAVAC – Compilador Java

O `javac` é o compilador da linguagem Java.

Sua função é transformar o código-fonte, escrito pelo programador, em bytecode.

O código-fonte possui a extensão `.java`, enquanto o bytecode gerado possui a extensão `.class`.

### Exemplo:

Código-fonte (`Programa.java`):

```java
public class Programa {
    public static void main(String[] args) {
        System.out.println("Olá, Java!");
    }
}
```

Para compilar o programa, utilizamos:

```bash
javac Programa.java
```

Após a compilação, será gerado o arquivo:

```text
Programa.class
```

Esse arquivo contém o bytecode que poderá ser executado pela JVM.

## 7. JVM – Java Virtual Machine

JVM significa **Java Virtual Machine**, ou Máquina Virtual Java.

É responsável por executar o bytecode gerado pelo compilador Java.

A JVM funciona como uma camada intermediária entre o programa Java e o sistema operacional.

### Principais funções da JVM

- Carregar os arquivos `.class`.
- Verificar o bytecode.
- Executar as instruções do programa.
- Gerenciar a memória.
- Realizar a coleta de lixo (Garbage Collection).
- Gerenciar recursos necessários durante a execução.

A JVM é fundamental para a portabilidade do Java, pois permite que o mesmo bytecode seja executado em diferentes sistemas operacionais por meio de máquinas virtuais compatíveis.

## 8. Como funciona o processo completo?

O funcionamento de uma aplicação Java pode ser representado pelas seguintes etapas:

1. O programador escreve o código-fonte em um arquivo `.java`.
2. O compilador `javac` transforma o código-fonte em bytecode.
3. O bytecode é armazenado em um arquivo `.class`.
4. A JVM carrega e executa o bytecode.
5. O programa é executado no sistema operacional.

### Representação do processo:

```text
        PROGRAMADOR
             |
             v
       CÓDIGO-FONTE
        Programa.java
             |
             v
        COMPILADOR
           JAVAC
             |
             v
          BYTECODE
        Programa.class
             |
             v
            JVM
    Java Virtual Machine
             |
             v
      SISTEMA OPERACIONAL
             |
             v
      PROGRAMA EXECUTADO
```

---

## 9. Resumo para revisão

| Conceito | Significado | Função |
|---|---|---|
| JDK | Java Development Kit | Desenvolver e executar aplicações Java. |
| JRE | Java Runtime Environment | Fornecer o ambiente de execução Java. |
| JVM | Java Virtual Machine | Executar o bytecode. |
| JAVAC | Java Compiler | Compilar o código-fonte Java. |
| WORA | Write Once, Run Anywhere | Escrever uma vez e executar em diferentes sistemas compatíveis. |
| Bytecode | Código intermediário | Código gerado após a compilação do programa Java. |

## 🎯 O que você precisa memorizar?

- JDK é o kit de desenvolvimento Java.
- JRE é o ambiente de execução Java.
- JVM é a máquina virtual responsável por executar o bytecode.
- JAVAC é o compilador Java.
- O arquivo `.java` contém o código-fonte.
- O arquivo `.class` contém o bytecode.
- WORA significa Write Once, Run Anywhere.
- A portabilidade do Java é possível graças ao bytecode e à JVM.
- O JDK permite desenvolver e executar aplicações Java.

## 🎯 Objetivo da aula

Compreender como funciona a plataforma Java, identificar as diferenças entre JDK e JRE e entender as funções do compilador JAVAC e da JVM no processo de compilação e execução de programas.
