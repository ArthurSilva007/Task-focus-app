# 📌 TaskFocus – Sistema de Gerenciamento de Tarefas e Finanças

<p align="center">
  <img src="https://user-images.githubusercontent.com/109287314/235314122-0941508f-287a-426c-85a6-06121f0e21a8.png" alt="TaskFocus Cover" width="800">
</p>

O **TaskFocus** é uma aplicação Full-Stack desenvolvida como projeto pessoal com o objetivo de centralizar o gerenciamento de tarefas e finanças de forma prática, intuitiva e segura. O sistema inclui um dashboard com gráficos interativos, autenticação com JWT, organização por prioridade e uma interface responsiva com suporte a tema claro/escuro.

---

## ✅ Funcionalidades Principais

- 🔐 **Autenticação e Autorização:** Sistema seguro com **JWT** e **Spring Security**.
- 📋 **CRUD Completo:** Gerenciamento total de tarefas e transações, com definição de prioridade e status.
- 📊 **Dashboard Interativo:** Gráficos dinâmicos (`Chart.js`) para acompanhar o progresso e as finanças.
- 🔎 **Filtros e Busca:** Ferramentas para encontrar tarefas rapidamente por título, status ou prioridade.
- 🌓 **Tema Dinâmico:** Suporte a modo escuro (Dark Mode) e claro (Light Mode) para maior conforto visual.
- ⏰ **Notificações:** Alertas visuais para tarefas importantes.
- 🏛️ **Arquitetura Robusta:** Estrutura separada por camadas no backend e frontend modularizado para garantir escalabilidade e manutenção.

---

## 🎨 Design e Prototipação

Toda a interface e a experiência do usuário (UX/UI) foram planejadas e prototipadas na ferramenta **Figma**, garantindo um fluxo de trabalho coeso antes do desenvolvimento.

---

## 🧰 Tecnologias Utilizadas

Este projeto foi construído utilizando um ecossistema moderno e robusto, tanto no backend quanto no frontend.

| Camada    | Tecnologias                                                              |
| :-------- | :----------------------------------------------------------------------- |
| 🎯 **Backend** | `Java 17`, `Spring Boot 3`, `Spring Security`, `JWT`, `JPA/Hibernate`, `PostgreSQL`, `Maven` |
| 💡 **Frontend** | `Angular 17` (Standalone), `TypeScript`, `RxJS`, `SCSS`, `Chart.js`, `Angular Material` |
| 🎨 **Design** | `Figma`                                                                  |

---

## 🏛️ Estrutura do Projeto

Backend (Spring Boot)

demo/
├── src/
│   └── main/
│       └── java/
│           └── Gestaodetarefa/
│               └── demo/
│                   ├── config/        # Configurações (Security, CORS, etc.)
│                   ├── auth/          # Controllers e DTOs de autenticação
│                   ├── model/         # Entidades JPA (User, Task)
│                   ├── repository/    # Repositórios Spring Data JPA
│                   ├── scheduler/     # Tarefas agendadas (ex: notificações)
│                   ├── service/       # Lógica de negócio
│                   └── TaskController/ # Controllers REST para as funcionalidades
├── resources/
└── application.properties # Configurações da aplicação


Frontend (Angular)

taskfocus-frontend/
├── src/
│   └── app/
│       ├── components/    # Componentes reutilizáveis (modal, header, etc.)
│       ├── guards/        # Guards de rota (auth.guard.ts)
│       ├── interceptors/  # Interceptadores HTTP (jwt.interceptor.ts)
│       ├── models/        # Interfaces e modelos de dados (task.model.ts)
│       ├── pages/         # Componentes de página (rotas principais)
│       ├── services/      # Serviços de comunicação com a API
│       └── app.routes.ts  # Definição das rotas da aplicação

---

## 🚀 Como Executar o Projeto

Para rodar o projeto localmente, você precisará ter o **Java 17 (JDK)**, **Maven**, **Node.js (v18+)** e o **Angular CLI** instalados.

### **Backend**

1.  Clone o repositório:
    ```bash
    git clone [https://github.com/ArthurSilva007/Task-focus-app.git](https://github.com/ArthurSilva007/Task-focus-app.git)
    ```
2.  Navegue até a pasta do backend:
    ```bash
    cd Task-focus-app/demo
    ```
3.  Configure seu banco de dados `PostgreSQL` local e atualize o arquivo `src/main/resources/application.properties` com suas credenciais.
4.  Execute a aplicação:
    ```bash
    mvn spring-boot:run
    ```
    O servidor backend estará rodando em `http://localhost:8080`.

### **Frontend**

1.  Navegue até a pasta do frontend em um novo terminal:
    ```bash
    cd Task-focus-app/taskfocus-frontend
    ```
2.  Instale as dependências:
    ```bash
    npm install
    ```
3.  Execute a aplicação:
    ```bash
    ng serve -o
    ```
    A aplicação abrirá automaticamente em `http://localhost:4200`.

---

## 👨‍💻 Autor

Feito com ❤️ por **Arthur Silva**.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-ArthurSilva-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/anderson-silva-15b340323/)
