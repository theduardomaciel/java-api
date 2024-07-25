# Beatstar Community API

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/.github/cover.png">
  <source media="(prefers-color-scheme: light)" srcset="/.github/cover_light.png">
  <img alt="Main project cover" src="/.github/cover_light.png">
</picture>

## 📝 Descrição

API RESTFul com Java e Spring Boot destinada ao funcionamento das plataformas (Android, Web) do, ainda em desenvolvimento, projeto Beatstar Community.

O projeto visa a criação de um ambiente em que a comunidade do jogo mobile Beatstar possa se reunião, compartilhando e descobrindo novas músicas enquanto interagem com outros usuários.

> [!NOTE]
> O design do frontend do projeto está disponível no [Figma](https://www.figma.com/design/2mWKQhZ8wsXQQEzBUDbFk5/Beatstar-Community?node-id=0-1&t=TP0OLPH97x2pLUsr-1)

## ✨ Tecnologias

- `[Base]` Java 22
- `[Framework]` Spring Boot 3.3.2
- `[Dependências]` Gradle

## 🏗️ Arquitetura

- **Controller:**  
  Utilizado para definir os endpoints da API  

- **Service:**  
  Utilizado para definir a lógica de negócio da aplicação

- **Repository:** 
  Utilizado para definir as operações de CRUD no banco de dados

- **Model:**  
  Utilizado para definir as entidades do banco de dados

- **DTO:**  
  Utilizado para não expor todos os campos das entidades do banco de dados diretamente

> **DTO** (Data Transfer Object) é um padrão de projeto cujo objetivo é transferir dados entre subsistemas de um software.  

## ☁️ Infraestrutura

- Banco de Dados: PostgreSQL
- Hospedagem: Railway
- ~~CI/CD: GitHub Actions~~

> **Procfile**: arquivo que informa ao Railway como iniciar a aplicação.

> [!WARNING]
> Caso o Railway falhe durante o deploy por conta da versão atual do Gradle ser muito recente, acesse o arquivo `gradle-wrapper.properties` presente em `gradle/wrapper` e altere a versão do Gradle para uma mais antiga.  
> 
> Exemplo:
> ```properties
> distributionUrl=https\://services.gradle.org/distributions/gradle-7.6.1-bin.zip
> ```

## 🚧 Roadmap

Este projeto ainda está em desenvolvimento e as próximas etapas consistem em:

- [ ] Implementar CRUD de usuários
- [ ] Implementar CRUD de charts
- [ ] Implementar CRUD de músicas
- [ ] Implementar CI/CD
- [ ] Documentar endpoints
- [ ] Implementar testes unitários
- [ ] Implementar testes de integração
- [ ] Implementar autenticação

## 📝 Licença

Este projeto utiliza a MIT License. Veja o arquivo de [LICENÇA](LICENSE) para mais detalhes.