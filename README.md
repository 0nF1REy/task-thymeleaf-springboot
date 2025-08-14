# Task Thymeleaf Spring Boot

Um sistema web elegante para gerenciamento de tarefas desenvolvido com Spring Boot e Thymeleaf, apresentando um design inspirado na estética italiana dos anos 1940-1950.

## 📋 Sobre o Projeto

Este é um sistema de gerenciamento de tarefas que permite criar, listar e editar tarefas com uma interface web moderna e responsiva. O projeto utiliza uma paleta de cores vintage e tipografia elegante para proporcionar uma experiência visual única.

## 🚀 Tecnologias Utilizadas

- **Java 21**
- **Spring Boot 3.5.4**
- **Spring Web**
- **Thymeleaf**
- **Spring DevTools**
- **Bootstrap 5.3.7**
- **Font Awesome**
- **Maven**

## 🏗️ Estrutura do Projeto

```
src/
├── main/
│   ├── java/br/com/alan/layout/
│   │   ├── LayoutApplication.java           # Classe principal
│   │   ├── controller/
│   │   │   ├── TaskController.java          # Controlador de tarefas
│   │   │   └── GlobalControllerAdvice.java  # Advice global
│   │   └── model/
│   │       └── Task.java                    # Modelo de tarefa
│   └── resources/
│       ├── static/css/
│       │   └── style.css                    # Estilos customizados
│       └── templates/
│           ├── create.html                  # Página de criação/edição
│           ├── list.html                    # Página de listagem
│           └── fragments.html               # Fragmentos reutilizáveis
└── test/
    └── java/br/com/alan/layout/
        └── LayoutApplicationTests.java      # Testes da aplicação
```

## 🎨 Características do Design

- **Paleta de Cores**: Inspirada na estética italiana vintage (preto profundo, dourado envelhecido, borgonha)
- **Tipografia**: Fontes elegantes (Crimson Text, Playfair Display)
- **Interface**: Design responsivo com gradientes e efeitos visuais sofisticados
- **Experiência**: Animações suaves e transições elegantes

## 🛠️ Funcionalidades

### ✅ Implementadas

- ✅ Cadastro de tarefas
- ✅ Listagem de tarefas
- ✅ Edição de tarefas
- ✅ Interface responsiva
- ✅ Navegação dinâmica com indicação de página ativa

### 📝 Modelo de Dados

A entidade [`Task`](src/main/java/br/com/alan/layout/model/Task.java) possui:

- `id`: Identificador único
- `name`: Nome da tarefa
- `date`: Data de execução (formato: dd/MM/yyyy HH:mm:ss)

## 🚀 Como Executar

### Pré-requisitos

- Java 21 ou superior
- Maven 3.6+ (ou use o wrapper incluído)

### Passos para execução

1. **Clone o repositório**

```bash
git clone <url-do-repositorio>
cd layout
```

2. **Execute com Maven Wrapper (recomendado)**

```bash
# Linux/macOS
./mvnw spring-boot:run

# Windows
mvnw.cmd spring-boot:run
```

3. **Ou compile e execute**

```bash
./mvnw clean compile
./mvnw spring-boot:run
```

4. **Acesse a aplicação**

- URL: `http://localhost:8080`
- A aplicação será iniciada na porta padrão 8080

## 🌐 Rotas da Aplicação

| Método | Rota         | Descrição                                         |
| ------ | ------------ | ------------------------------------------------- |
| `GET`  | `/create`    | Exibe formulário de criação de tarefa             |
| `POST` | `/create`    | Processa criação/atualização de tarefa            |
| `GET`  | `/list`      | Exibe lista de tarefas                            |
| `GET`  | `/edit/{id}` | Exibe formulário de edição para tarefa específica |

## 🎯 Navegação

- **Cadastro**: Permite criar novas tarefas ou editar existentes
- **Listagem**: Exibe todas as tarefas com opção de edição

## 📱 Responsividade

O sistema é totalmente responsivo com breakpoints para:

- **Desktop**: > 768px
- **Tablet**: ≤ 768px
- **Mobile**: ≤ 480px

## 🧪 Testes

Execute os testes com:

```bash
./mvnw test
```

## 📦 Build para Produção

```bash
./mvnw clean package
java -jar target/layout-0.0.1-SNAPSHOT.jar
```

## 🔧 Configuração

As configurações estão no arquivo [`application.properties`](src/main/resources/application.properties):

```properties
spring.application.name=layout
```

## 👨‍💻 Desenvolvimento

### Estrutura dos Controladores

- [`TaskController`](src/main/java/br/com/alan/layout/controller/TaskController.java): Gerencia operações CRUD de tarefas
- [`GlobalControllerAdvice`](src/main/java/br/com/alan/layout/controller/GlobalControllerAdvice.java): Adiciona URI atual a todos os modelos

### Armazenamento

**Nota**: Este projeto utiliza armazenamento em memória (List) para fins de demonstração. Em produção, considere integrar com banco de dados.

## 🎨 Personalização de Estilos

O arquivo [`style.css`](src/main/resources/static/css/style.css) contém toda a estilização customizada com:

- Variáveis CSS para cores temáticas
- Gradientes e sombras
- Animações e transições
- Responsividade completa

## 👤 Sobre o Desenvolvedor

<div align="center">

<table>
  <tr>
    <td align="center">
        <br>
        <a href="https://github.com/0nF1REy" target="_blank">
          <img src="./readme_images/alan-ryan.jpg" height="160" alt="Foto de Alan Ryan" style="border-radius:50%;border:3px solid #0077B5;">
        </a>
        </p>
        <a href="https://github.com/0nF1REy" target="_blank">
          <strong>Alan Ryan</strong>
        </a>
        </p>
        ☕ Peopleware | Tech Enthusiast | Code Slinger ☕
        <br>
        Apaixonado por código limpo, arquitetura escalável e experiências digitais envolventes
        </p>
          Conecte-se comigo:
        </p>
        <a href="https://www.linkedin.com/in/alan-ryan-b115ba228" target="_blank">
          <img src="https://img.shields.io/badge/LinkedIn-Alan_Ryan-0077B5?style=flat&logo=linkedin" alt="LinkedIn">
        </a>
        <a href="https://gitlab.com/alanryan619" target="_blank">
          <img src="https://img.shields.io/badge/GitLab-@0nF1REy-FCA121?style=flat&logo=gitlab" alt="GitLab">
        </a>
        <a href="mailto:alanryan619@gmail.com" target="_blank">
          <img src="https://img.shields.io/badge/Email-alanryan619@gmail.com-D14836?style=flat&logo=gmail" alt="Email">
        </a>
        </p>
    </td>
  </tr>
</table>

</div>

---

## 📫 Contribuir

Contribuições são muito bem-vindas! Se você deseja contribuir com o projeto, por favor, siga estes passos:

1.  **Faça um Fork** do repositório.

2.  **Crie uma nova Branch** para sua feature ou correção:

    ```bash
    git checkout -b feature/nome-da-feature
    ```

3.  **Faça suas alterações** e realize o commit:

    ```bash
    git commit -m "feat: Adiciona nova feature"
    ```

4.  **Envie suas alterações** para o seu fork:

    ```bash
    git push origin feature/nome-da-feature
    ```

5.  **Abra um pull request** para a branch `main` do repositório original.

## 📚 Recursos Adicionais

- **<a href="https://www.atlassian.com/br/git/tutorials/making-a-pull-request" target="_blank">📝 Como criar um Pull Request</a>**

- **<a href="https://www.conventionalcommits.org/en/v1.0.0/" target="_blank">💾 Padrão de Commits Convencionais</a>**

## 📜 Licença

Este projeto é um projeto de demonstração desenvolvido para fins educacionais.

⭐ Se este repositório foi útil para você, considere dar uma estrela!
