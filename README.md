# 💻 Java Clean Architecture Playground

![Java](https://img.shields.io/badge/Java-25-orange)
![Status](https://img.shields.io/badge/Status-In%20Progress-blue)
![DIO](https://img.shields.io/badge/DIO-Project-blueviolet)

> Hands-on Java project exploring Clean Code, SOLID principles, Object Calisthenics, Design Patterns (Strategy & Factory), Data Structures and Clean Architecture using modern Java (Java 25).

---

## 🎓 Projeto desenvolvido para

Desafio de Projeto da DIO utilizando o **NotebookLM** como ferramenta de aprendizagem ativa, engenharia de prompts e construção de conhecimento técnico.

---

## 📌 Contexto e Objetivos

Este repositório foi desenvolvido com foco em aprendizagem ativa utilizando Inteligência Artificial (NotebookLM), combinando teoria e prática para evolução como desenvolvedor backend Java.

### 🎯 Objetivos de estudo

* Escrever código limpo e legível
* Aplicar princípios SOLID
* Utilizar Object Calisthenics na prática
* Implementar Design Patterns
* Trabalhar com Estruturas de Dados
* Estruturar aplicações com Clean Architecture
* Utilizar recursos modernos do Java (Java 25)

---

## 📚 Curadoria de Fontes

### Livros

* 📘 *Clean Code* — Robert C. Martin
* 📘 *Clean Architecture* — Robert C. Martin
* 📘 *Effective Java* — Joshua Bloch

### Sites e Documentação

- 🌐 [Refactoring Guru](https://refactoring.guru/)
- 🌐 [Oracle Java Documentation](https://docs.oracle.com/en/java/)
* 📄 Materiais e anotações da DIO

---

## 🧠 Engenharia de Prompts e Aprendizados ("Cicatrizes")

Durante os estudos utilizando o NotebookLM, foram realizados diversos experimentos para entender como diferentes formas de formular perguntas influenciam a qualidade das respostas geradas pela IA.

---

### Caso 1 — Comparando Clean Code, SOLID e Object Calisthenics

#### Prompt

```text
Explique as diferenças entre Clean Code, SOLID e Object Calisthenics. Quando devo aplicar cada um deles em projetos Java?
```

#### Resultado Obtido

A IA apresentou uma comparação clara entre os três conceitos:

* Clean Code → foco na legibilidade e manutenção do código.
* SOLID → foco na organização das classes e dependências.
* Object Calisthenics → conjunto de exercícios para desenvolver melhores práticas de orientação a objetos.

#### Aprendizado

Percebi que os três conceitos são complementares e atuam em níveis diferentes do desenvolvimento de software.

#### Fontes Utilizadas

* Clean Code (Robert C. Martin)
* Clean Architecture (Robert C. Martin)
* Object Calisthenics (Jeff Bay)

---

### Caso 2 — Problemas causados pela ausência do SOLID

#### Prompt

```text
Quais problemas de manutenção podem ocorrer quando os princípios SOLID não são aplicados?
```

#### Resultado Obtido

A IA apresentou problemas comuns encontrados em sistemas legados:

* Classes com múltiplas responsabilidades
* Acoplamento excessivo
* Dificuldade para testes unitários
* Necessidade de modificar código existente para adicionar novas funcionalidades
* Propagação de bugs em diferentes módulos

#### Aprendizado

Entendi que SOLID não existe apenas para "deixar o código bonito", mas para reduzir o custo de manutenção e evolução do software.

#### Fontes Utilizadas

* Clean Architecture
* Refactoring Guru

---

### Caso 3 — Refatoração prática utilizando SOLID

#### Prompt

```text
Mostre exemplos em Java que violam cada princípio SOLID e apresente uma versão refatorada.
```

#### Resultado Obtido

A IA apresentou exemplos práticos para:

* SRP
* OCP
* LSP
* ISP
* DIP

Incluindo versões problemáticas e versões refatoradas utilizando boas práticas.

#### Aprendizado

Exemplos práticos facilitaram muito mais a compreensão dos princípios do que apenas definições teóricas.

#### Fontes Utilizadas

* Clean Architecture
* Refactoring Guru

---

### Caso 4 — Design Pattern Strategy

#### Prompt

```text
Como o padrão Strategy ajuda a reduzir estruturas condicionais complexas?
```

#### Resultado Obtido

A IA demonstrou como substituir cadeias de `if/else` e `switch/case` por polimorfismo.

Também relacionou o padrão Strategy com o princípio Open/Closed Principle (OCP).

#### Aprendizado

Compreendi como o Strategy ajuda a manter o código aberto para extensão e fechado para modificação.

#### Fontes Utilizadas

* Refactoring Guru
* Clean Architecture

---

### Caso 5 — Object Calisthenics aplicado ao Backend Java

#### Prompt

```text
Analise as regras de Object Calisthenics e identifique quais delas trazem maior benefício para aplicações backend Java.
```

#### Resultado Obtido

As regras destacadas como mais relevantes foram:

* Evitar `else`
* Encapsular primitivos e coleções
* Aplicar Tell, Don't Ask
* Evitar excesso de getters e setters

#### Aprendizado

Percebi que Object Calisthenics pode ser utilizado como um exercício para desenvolver um design mais orientado a objetos e complementar os princípios SOLID.

#### Fontes Utilizadas

* Object Calisthenics (Jeff Bay)
* Clean Code

---

### 🔧 Dificuldades Encontradas (Troubleshooting)

| Problema                                         | Solução                                  |
| ------------------------------------------------ | ---------------------------------------- |
| Prompts genéricos geravam respostas superficiais | Tornar os prompts mais específicos       |
| Respostas muito teóricas                         | Solicitar exemplos em Java               |
| Conceitos difíceis de visualizar                 | Pedir refatorações passo a passo         |
| Explicações isoladas                             | Relacionar conceitos com problemas reais |

---

### 🎯 Conclusão

A principal lição aprendida durante o uso do NotebookLM foi que a qualidade das respostas está diretamente relacionada à qualidade dos prompts utilizados.

Perguntas mais específicas, contextualizadas e orientadas para exemplos práticos produziram respostas significativamente mais úteis para o aprendizado e aplicação dos conceitos em projetos Java.

---

## 📘 Miniguia de Estudo

### 🧹 Clean Code

#### Boas práticas

* Nomes claros e descritivos
* Métodos pequenos
* Baixo acoplamento
* Alta coesão
* Evitar comentários desnecessários

```java
// ❌ Ruim
int d;

// ✅ Bom
int diasTrabalhados;
```

---

### 🧱 SOLID

* **S** — Single Responsibility Principle
* **O** — Open/Closed Principle
* **L** — Liskov Substitution Principle
* **I** — Interface Segregation Principle
* **D** — Dependency Inversion Principle

---

### 🧠 Object Calisthenics

Conjunto de regras para incentivar código mais limpo e orientado a objetos.

#### Principais regras

* Um nível de indentação por método
* Evitar uso de `else`
* Encapsular coleções
* Classes pequenas
* Nomes descritivos
* Evitar getters e setters desnecessários

#### Exemplo

```java
if (usuario != null) {
    if (usuario.isAtivo()) {
        processar(usuario);
    }
}
```

Refatoração:

```java
validarUsuario(usuario);
processar(usuario);
```

---

### 🧩 Design Patterns

#### Strategy

Permite trocar comportamentos dinamicamente.

```java
interface DescontoStrategy {
    double calcular(double valor);
}
```

#### Factory

Centraliza a criação de objetos.

```java
class NotificacaoFactory {

    public static Notificacao criar(String tipo) {

        if (tipo.equals("email")) return new Email();

        if (tipo.equals("sms")) return new SMS();

        throw new IllegalArgumentException();
    }
}
```

---

### 📊 Estruturas de Dados

* Array
* List
* Stack
* Queue
* Map

📌 Saber quando utilizar cada estrutura é mais importante do que memorizar sua implementação.

---

### 🏗️ Clean Architecture

Camadas principais:

* Domain
* Use Cases
* Adapters
* Infrastructure

#### Benefícios

* Baixo acoplamento
* Alta testabilidade
* Facilidade de manutenção
* Independência de frameworks

---

### ☕ Java 25

Principais recursos estudados:

* Melhorias de performance
* Pattern Matching
* Virtual Threads (Project Loom)
* Código mais expressivo
* Evolução contínua da linguagem

---

## 📖 Glossário

| Conceito       | Definição                                         |
| -------------- | ------------------------------------------------- |
| Acoplamento    | Dependência entre classes                         |
| Coesão         | Responsabilidade única e bem definida             |
| Refatoração    | Melhoria interna sem alterar comportamento        |
| Design Pattern | Solução reutilizável para problemas recorrentes   |
| OCP            | Aberto para extensão e fechado para modificação   |
| DIP            | Dependência de abstrações e não de implementações |

---

## 🔁 Prompts Reutilizáveis

```text
Explique X com exemplos em Java
```

```text
Refatore esse código aplicando boas práticas
```

```text
Esse código segue SOLID?
```

```text
Qual Design Pattern resolve esse problema?
```

```text
Como aplicar Object Calisthenics neste código?
```

```text
Como transformar esse código em uma arquitetura mais aderente ao Clean Architecture?
```

---

## 🚀 Estrutura do Projeto

```bash
src/
 ├── domain/
 ├── usecase/
 ├── adapter/
 └── infrastructure/
```

---

## 🛠️ Tecnologias

* Java 25
* Programação Orientada a Objetos
* SOLID
* Object Calisthenics
* Design Patterns
* Clean Architecture

---

## 🔗 Como executar

```bash
git clone https://github.com/flavioReisSouza/java-clean-architecture-playground.git
```

---

## 🏆 Resultado do Projeto

Este projeto foi desenvolvido como parte do desafio da DIO utilizando o NotebookLM como ferramenta de aprendizagem ativa.

Durante o desenvolvimento foram estudados e consolidados conceitos fundamentais para aplicações backend Java modernas:

* Clean Code
* SOLID
* Object Calisthenics
* Design Patterns (Strategy e Factory)
* Estruturas de Dados
* Clean Architecture
* Java 25

Além do aprofundamento técnico, o projeto também permitiu praticar:

* Curadoria de fontes técnicas
* Engenharia de Prompts
* Troubleshooting de respostas geradas por IA
* Organização do conhecimento
* Documentação técnica

O resultado final é um material de consulta que poderá ser reutilizado futuramente em entrevistas, estudos e projetos profissionais.

---

## 👨‍💻 Autor

**Flávio Reis Souza**

Backend Java Developer | Estudante de Ciência da Computação | Entusiasta de Arquitetura de Software, Boas Práticas e Clean Code.

🔗 GitHub: https://github.com/flavioReisSouza
