# Spring IoC para .NET

➡️ Curso relacionado: **[Spring IoC para .NET](https://stahe.github.io/br-springioc-dotnet-avril-2005/)**

Este documento apresenta os princípios da **inversão de controle (IoC)** e sua implementação no ecossistema **.NET** por meio do framework **Spring.NET**, uma adaptação do framework **Spring** originalmente projetado para Java. 

O objetivo é mostrar como o projeto de aplicativos pode ser aprimorado ao **desacoplar componentes** e deixar que um contêiner de configuração se encarregue de sua composição.

---

# Objetivos deste documento

Este tutorial tem os seguintes objetivos:

- explorar as possibilidades de **configuração e integração do framework Spring** em uma aplicação .NET  
- compreender o conceito de **Inversão de Controle (IoC)**  
- aprender como a **injeção de dependências (Dependency Injection)** pode ser usada para desacoplar componentes  
- aplicar esses conceitos em **exemplos concretos em VB.NET** 

---

# Contexto

As ideias apresentadas neste documento são fortemente inspiradas no livro de **Rod Johnson**:

**J2EE Development without EJB (Wrox, 2004)**

Este livro lançou as bases para a filosofia do Spring: construir aplicações mais simples, mais modulares e mais fáceis de testar, evitando dependências pesadas de frameworks tradicionais.

Já existe um documento semelhante para **Spring / Java**.  
Este tutorial retoma os mesmos conceitos e **os adapta à plataforma .NET**. 

---

# Spring.NET

No momento da redação deste documento:

- o **Spring.NET** está disponível na versão **0.6 RC3 (abril de 2005)**  
- apenas algumas funcionalidades do Spring Java original foram portadas  
- no entanto, as funcionalidades essenciais estão disponíveis:

- **Inversão de Controle (IoC)**
- **Programação Orientada a Aspectos (AOP)**

Este tutorial enfoca principalmente o **IoC**, que constitui o cerne da filosofia do Spring. 

---

# Princípio: Inversão de Controle (IoC)

Em uma arquitetura clássica:

- um objeto cria suas próprias dependências;
- o objeto controla diretamente os objetos de que necessita;

Com **IoC**:

- as dependências são **injetadas por um contêiner**;
- os componentes são **fracamente acoplados**
- a configuração é **externalizada**

Isso garante:

- uma **melhor manutenção**
- uma **maior testabilidade**
- uma **arquitetura mais flexível**

---

# Exemplos práticos

A parte prática do documento contém diversos exemplos que ilustram o seguinte:

- a configuração de componentes do Spring.NET
- a injeção de dependências
- a criação de objetos de negócio desacoplados

Os exemplos foram escritos em **VB.NET**.

Os testes utilizam o framework **NUnit**, o equivalente em .NET ao framework **JUnit** usado no ecossistema Java. 

---

# Requisitos

Para acompanhar os exemplos:

- Ambiente **.NET**
- **Spring.NET**
- **NUnit** para a execução de testes unitários

Nos anexos do documento, é explicado:

- onde essas ferramentas podem ser baixadas
- como devem ser instaladas

---

# Filosofia do Spring

A principal vantagem do Spring não reside apenas nos mecanismos técnicos, mas sobretudo na **filosofia de projeto**:

- separação de responsabilidades  
- acoplamento fraco entre componentes  
- configuração externa de dependências  
- arquitetura orientada a testes

Esses princípios permitem projetar aplicações **mais simples, mais modulares e mais robustas**.

