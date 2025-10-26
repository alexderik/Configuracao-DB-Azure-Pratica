# Configurando uma Instância de Banco de Dados na Azure

## 🚀 Introdução

Este repositório documenta a experiência prática de configuração de uma instância de **Azure SQL Database** (PaaS) na plataforma Microsoft Azure, como parte do desafio proposto pela Digital Innovation One (DIO). O objetivo foi aplicar os conceitos de serviços gerenciados na nuvem, focando na criação e documentação de um Banco de Dados SQL de forma clara e estruturada.

---

## ⚙️ Configuração na Azure: Passo a Passo

O banco de dados escolhido foi o **Azure SQL Database**, a solução PaaS (Plataforma como Serviço) totalmente gerenciada da Microsoft.

### 1. Preparação e Criação do Servidor Lógico

Antes de criar o banco de dados, foi necessário definir o ambiente lógico no Azure.

| Configuração | Detalhes da Configuração |
| :--- | :--- |
| **Grupo de Recursos** | `RG-DIO-SQL-Desafio` (Criado para isolamento e gerenciamento dos recursos). |
| **Servidor Lógico** | `desafioserverXXXX` (Novo servidor lógico, o ponto de acesso para o banco). |
| **Login do Administrador** | `Alexderik` |
| **Localização** | `Brazil South` (Região escolhida). |

### 2. Configuração do Banco de Dados e Tier de Serviço

Esta etapa define o nome do banco, o modelo de computação e o custo.

* **Nome do Banco de Dados:** `MeuPrimeiroDB`
* **Modelo de Computação:** **Uso Geral - Sem Servidor (Serverless)**
    * **Vantagem:** Este modelo oferece escalabilidade automática e cobra apenas pelo uso ativo (por vCore/segundo), sendo ideal para ambientes de desenvolvimento e cargas de trabalho intermitentes.
* **vCores:** 1 vCore
* **Armazenamento Máximo:** 32 GB

**(Aqui você deve inserir a imagem da Revisão Final / Custo estimado):**
```markdown
![Configuração de Revisão e Custo](images/01-Revisao-Custo.png)
