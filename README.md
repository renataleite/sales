# SalesWebMvc

## Descrição

O projeto SalesWebMvc é uma aplicação web ASP.NET Core MVC que gerencia vendas de uma empresa fictícia. A aplicação permite operações CRUD (Criar, Ler, Atualizar, Deletar) em departamentos, vendedores e registros de vendas.

## Funcionalidades

- **Gerenciamento de Departamentos**: Criação, visualização, edição e exclusão de departamentos.
- **Gerenciamento de Vendedores**: Criação, visualização, edição e exclusão de vendedores.
- **Registros de Vendas**: Pesquisa simples e agrupada por datas, além de operações CRUD em registros de vendas.

## Tecnologias Utilizadas

- ASP.NET Core MVC
- Entity Framework Core
- MySQL (via Pomelo.EntityFrameworkCore.MySql)
- Bootstrap para estilização

## Configuração do Projeto

### Pré-requisitos

- .NET 5.0 SDK ou superior
- MySQL Server
- Visual Studio ou editor de código de sua preferência (VSCode, por exemplo)

### Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/renataleite/SalesWebMvc.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd SalesWebMvc
   ```
3. Restaure os pacotes NuGet:
   ```bash
   dotnet restore
   ```
4. Ajuste a string de conexão para o MySQL no arquivo `appsettings.json`, conforme sua configuração local.

5. Execute as migrações para criar o banco de dados:
   ```bash
   dotnet ef database update
   ```

### Execução

Para rodar o projeto localmente, execute o seguinte comando no diretório do projeto:
```bash
dotnet run
```
Acesse a aplicação via navegador no endereço [http://localhost:5000](http://localhost:5000).

## Estrutura de Diretórios

- **Controllers**: Contém os controladores que gerenciam a lógica de interação com o usuário.
- **Models**: Inclui as classes de modelo que representam as entidades do banco de dados.
- **Views**: Contém as páginas .cshtml que são renderizadas ao usuário.
- **Services**: Camada de serviço para abstração da lógica de negócios.
- **Data**: Configurações de contexto do Entity Framework.

## Contribuição

Contribuições são sempre bem-vindas! Por favor, leia o arquivo CONTRIBUTING.md para detalhes sobre o nosso código de conduta, e o processo para enviar pull requests.
