# 📢 NewsFlash API

## 📄 **Descrição do Projeto**
A **NewsFlash API** é uma aplicação desenvolvida em **Java 17** usando **Spring WebFlux** para fornecer notícias em tempo real e enviar notificações personalizadas de breaking news por meio do **Apache Kafka**. O objetivo do projeto é demonstrar o uso de tecnologias modernas para criar uma API escalável e performática.

---

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

## 🤝 **Contribuição**
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.

---

## 📄 **Licença**
Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## ✨ **Autor**
- **Wallace Gonçalves**
- [GitHub](https://github.com/wcosme)
- [LinkedIn](https://www.linkedin.com/in/wcosme/)

API para envio de notícias em tempo real usando Spring WebFlux e Kafka.
