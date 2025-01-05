# 📢 NewsFlash API

## 📄 **Descrição do Projeto**
A **NewsFlash API** é uma aplicação desenvolvida em **Java 17** usando **Spring WebFlux** com o objetivo de fornecer notificações em tempo real de notícias relevantes. O projeto foi criado para praticar conceitos de APIs reativas, **Kafka**, **Redis**, e **arquitetura hexagonal**, com suporte completo para conteinerização.

---

## 🎯 **Objetivo do Projeto**

O objetivo principal do NewsFlash API é permitir que usuários recebam notícias personalizadas e notificações em tempo real através de um sistema escalável e performático. A aplicação consome dados de uma API externa de notícias e utiliza Kafka para enviar alertas de breaking news.


## 🛠️ **Tecnologias Utilizadas**
- **Java 17**
- **Spring Boot 3.1.2**
- **Spring WebFlux**
- **MongoDB**
- **Redis**
- **Apache Kafka**
- **Docker**
- **Lombok**
- **ModelMapper**
- **JUnit 5**
- **Mockito**

---

## 📦 **Arquitetura do Projeto**
O projeto foi desenvolvido utilizando a **Arquitetura Hexagonal**, garantindo uma separação clara de responsabilidades e facilitando a manutenção e escalabilidade.

- **Core (Domínio)**: Contém as regras de negócio.
- **Adapters (Portas e Adaptadores)**: Integrações com banco de dados, cache, mensageria e APIs externas.
- **Application (Camada de Aplicação)**: Endpoints REST e configuração da aplicação.

---

## 📦 Estrutura do Projeto
O projeto segue a **arquitetura hexagonal**, que facilita a separação de responsabilidades e garante flexibilidade na manutenção e evolução da aplicação.

```
newsflash-api
├── adapters
│   ├── in
│   └── out
├── application
│   └── services
├── domain
├── infrastructure
└── README.md
```

## 📋 **Funcionalidades**
- 📑 **Consulta de notícias em tempo real** via API externa.
- 🔔 **Criação de alertas personalizados** para notificações de breaking news.
- 📦 **Cache de respostas** com Redis para otimizar a performance.
- 📊 **Notificações em tempo real** utilizando Apache Kafka.

---

## 📚 **Como Executar o Projeto**

### 🔧 **Pré-requisitos**
Certifique-se de ter instalado:
- **Java 17**
- **Docker**
- **MongoDB**
- **Redis**
- **Apache Kafka**

### 🚀 **Passos para Rodar o Projeto**
1. Clone o repositório:
   ```bash
   git clone https://github.com/wcosme/newsflash-api.git
   ```

2. Navegue até a pasta do projeto:
   ```bash
   cd newsflash-api
   ```

3. Execute o projeto com Maven:
   ```bash
   ./mvnw spring-boot:run
   ```

4. Acesse a aplicação em:
   ```
   http://localhost:8080
   ```

---

## 🐳 **Conteinerização**
Este projeto já está preparado para ser executado em containers usando **Docker**.

### 📦 **Build da Imagem Docker**
```bash
docker build -t newsflash-api .
```

### 🏃 **Executar o Container**
```bash
docker run -p 8080:8080 newsflash-api
```

---

## 📑 **Documentação da API**
A documentação da API está disponível em **Swagger** após a execução do projeto:
```text
http://localhost:8080/swagger-ui/index.html
```

---

## 🧪 **Testes**
Os testes unitários foram escritos usando **JUnit 5** e **Mockito**. Para rodar os testes, use o comando:
```bash
./mvnw test
```

---

## 🤝 Como Contribuir
Contribuições são bem-vindas! Siga os passos abaixo para contribuir:
1. Faça um fork do projeto.
2. Crie uma branch com sua feature: `git checkout -b minha-feature`.
3. Commit suas alterações: `git commit -m 'Adiciona minha feature'`.
4. Faça um push para a branch: `git push origin minha-feature`.
5. Abra um Pull Request.
---

## 📄 **Licença**
Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## ✨ **Autor**
- **Wallace Gonçalves**
- [GitHub](https://github.com/wcosme)
- [LinkedIn](https://www.linkedin.com/in/wcosme/)

API para envio de notícias em tempo real usando Spring WebFlux e Kafka.