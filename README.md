# 💻 Java Clean Architecture Playground

> Hands-on Java project exploring Clean Code, SOLID principles, Object Calisthenics, Design Patterns (Strategy & Factory), Data Structures and Clean Architecture using modern Java (Java 25).

---

## 📌 Contexto e Objetivos

Este repositório foi desenvolvido com foco em aprendizagem ativa utilizando Inteligência Artificial (NotebookLM), combinando teoria e prática para evolução como desenvolvedor backend Java.

### 🎯 Objetivos de estudo

- Escrever código limpo e legível  
- Aplicar princípios SOLID  
- Utilizar Object Calisthenics na prática  
- Implementar Design Patterns  
- Trabalhar com estruturas de dados  
- Estruturar aplicações com Clean Architecture  
- Utilizar recursos modernos do Java (Java 25)  

---

## 📚 Curadoria de Fontes

- 📘 *Clean Code* — Robert C. Martin  
- 📘 *Effective Java* — Joshua Bloch  
- 🌐 Refactoring Guru — https://refactoring.guru/
- 🌐 Oracle Java Documentation — https://docs.oracle.com/en/java/
- 📄 Documentação oficial do Java (Oracle)  
- 📄 Materiais e anotações da DIO  

---

## 🧠 Engenharia de Prompts e Aprendizados ("Cicatrizes")

Durante os estudos utilizando o NotebookLM, foram realizados diversos experimentos para entender como diferentes formas de formular perguntas influenciam a qualidade das respostas geradas pela IA.

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

* Classes com múltiplas responsabilidades.
* Acoplamento excessivo.
* Dificuldade para testes unitários.
* Necessidade de modificar código existente para adicionar novas funcionalidades.
* Propagação de bugs em diferentes módulos.

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

Também relacionou o padrão Strategy com o princípio Open/Closed (OCP).

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

A principal lição aprendida durante o uso do NotebookLM foi que a qualidade das respostas está diretamente relacionada à qualidade dos prompts utilizados. Perguntas mais específicas, contextualizadas e orientadas para exemplos práticos produziram respostas significativamente mais úteis para o aprendizado e aplicação dos conceitos em projetos Java.


---

## 📘 Miniguia de Estudo

### 🧹 Clean Code

Boas práticas:

- Nomes claros e descritivos  
- Métodos pequenos  
- Baixo acoplamento  
- Alta coesão  
- Evitar comentários desnecessários  

```java
// ❌ Ruim
int d;

// ✅ Bom
int diasTrabalhados;
```

---

### 🧱 SOLID

- **S** — Single Responsibility Principle  
- **O** — Open/Closed Principle  
- **L** — Liskov Substitution Principle  
- **I** — Interface Segregation Principle  
- **D** — Dependency Inversion Principle  

---

### 🧠 Object Calisthenics

Conjunto de regras para incentivar código mais limpo e orientado a objetos.

#### 📌 Principais regras

- Um nível de indentação por método  
- Evitar uso de `else`  
- Encapsular coleções  
- Classes pequenas  
- Nomes descritivos  
- Evitar getters/setters desnecessários  

#### 💡 Exemplo prático

❌ Código com alta complexidade:

```java
if (usuario != null) {
    if (usuario.isAtivo()) {
        processar(usuario);
    }
}
```

✅ Código mais limpo:

```java
validarUsuario(usuario);
processar(usuario);
```

---

### 🧩 Design Patterns

#### 🔹 Strategy

Permite trocar comportamentos dinamicamente.

```java
interface DescontoStrategy {
    double calcular(double valor);
}
```

---

#### 🔹 Factory

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

- Array  
- List  
- Stack  
- Queue  
- Map  

📌 Saber quando usar é mais importante que decorar  

---

### 🏗️ Clean Architecture

Divisão em camadas:

- Domain  
- Use Cases  
- Adapters  
- Infrastructure  

📌 Benefícios:

- Baixo acoplamento  
- Alta testabilidade  
- Manutenção facilitada  

---

### ☕ Java 25

- Melhorias de performance  
- Pattern Matching  
- Virtual Threads (Project Loom)  
- Código mais expressivo  

---

## 📖 Glossário

- **Acoplamento** → dependência entre classes  
- **Coesão** → responsabilidade única  
- **Refatoração** → melhoria sem alterar comportamento  
- **Design Pattern** → solução reutilizável  

---

## 🔁 Prompts Reutilizáveis

- "Explique X com exemplos em Java"  
- "Refatore esse código aplicando boas práticas"  
- "Esse código segue SOLID?"  
- "Qual Design Pattern resolve esse problema?"  

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

- Java 25  
- Programação Orientada a Objetos  
- Design Patterns  
- Clean Architecture

## 🔗 Como executar

```bash
git clone https://github.com/flavioReisSouza/java-clean-architecture-playground
```
