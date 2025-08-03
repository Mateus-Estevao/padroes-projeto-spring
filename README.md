# 🚀 Explorando Padrões de Projetos na Prática com Java

Este repositório contém as implementações dos **padrões de projeto** explorados no Lab **"Explorando Padrões de Projetos na Prática com Java"**, utilizando o **Spring Framework** para estruturar as soluções de forma robusta e escalável.

## 📋 Descrição

O projeto tem como objetivo demonstrar, de forma prática, a aplicação de alguns dos principais padrões de projeto no desenvolvimento de aplicações Java. Foram implementados exemplos práticos que simulam cenários do mundo real, permitindo entender como cada padrão resolve problemas recorrentes de design de software.

## 🛠️ Padrões de Projeto Utilizados

### 1. 🟢 Singleton
O padrão **Singleton** garante que uma classe tenha apenas uma instância, e fornece um ponto global de acesso a ela.

**Aplicações:**
- Controle de instância única de serviços no Spring.
- Beans do Spring são Singleton por padrão, demonstrando como o framework gerencia o ciclo de vida das instâncias.

---

### 2. 🧩 Strategy / Repository
O padrão **Strategy** permite definir uma família de algoritmos, encapsulá-los e torná-los intercambiáveis.

O padrão **Repository** centraliza a lógica de acesso a dados, separando a camada de persistência do restante da aplicação.

**Aplicações:**
- Implementação de diferentes estratégias de busca ou cálculo de valores.
- Criação de interfaces de repositórios (utilizando Spring Data JPA) para abstrair a persistência dos dados.
- Permite alterar facilmente a estratégia de execução via injeção de dependência do Spring.

---

### 3. 🏢 Facade
O padrão **Facade** fornece uma interface simplificada para um subsistema mais complexo, ocultando as complexidades internas.

**Aplicações:**
- Criação de uma camada de serviço que orquestra múltiplas chamadas de repositórios ou serviços externos.
- Redução do acoplamento entre controladores e as regras de negócio complexas.

---

## 🖥️ Tecnologias Utilizadas
- Java 17+
- Spring Boot
- Spring Framework (IoC/DI)
- Spring Data JPA (para abstração de repositórios)
- H2 Database (banco em memória para testes)
- Lombok (para redução de boilerplate code)
- Maven (gerenciamento de dependências)

---

## 📂 Estrutura do Projeto
src/

└── main/
└── java/
└── br/
└── com/
└── dio/
└── patterns/
├── singleton/
├── strategy/
├── repository/
├── facade/
└── Application.java

---

## ▶️ Como Executar o Projeto

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/SeuUsuario/explorando-padroes-java.git
Navegue até o diretório do projeto:


cd explorando-padroes-java
Execute a aplicação:


./mvnw spring-boot:run
ou, caso esteja utilizando IntelliJ/Eclipse: Execute a classe Application.java.

Acesse no navegador:


http://localhost:8080

## 🎯 Objetivos do Projeto

Entender o papel dos padrões de projeto na organização e manutenibilidade do código.

Explorar a implementação prática de padrões com apoio do ecossistema Spring.

Demonstrar como o uso correto de padrões contribui para um código mais limpo, flexível e desacoplado.

📚 Referências
Design Patterns - GoF

Documentação Oficial Spring

DIO - Digital Innovation One

🤝 Contribuição
Contribuições são bem-vindas! Fique à vontade para abrir issues, pull requests ou sugerir melhorias.

📄 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.



Quer que eu crie também um exemplo de código para cada padrão (Singleton, Strategy, Repository, Facad