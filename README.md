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
- 🌐 https://refactoring.guru/  
- 📄 Documentação oficial do Java (Oracle)  
- 📄 Materiais e anotações da DIO  

---

## 🧠 Engenharia de Prompts e Aprendizados

### 🔹 Prompt genérico

```
Explique SOLID
```

❌ Superficial e pouco prático

---

### 🔹 Prompt refinado

```
Explique SOLID com exemplos em Java e problemas reais
```

✅ Respostas mais úteis e aplicáveis

---

### 🔹 Prompt prático

```
Refatore esse código aplicando SOLID
```

🔥 Aprendizado mais efetivo

---

### 🔹 Prompt de análise

```
Esse código viola algum princípio SOLID?
```

💡 Excelente para troubleshooting

---

### 📌 Insight principal

A qualidade da resposta da IA depende diretamente da qualidade do prompt.

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
