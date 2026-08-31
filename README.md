# Inventory-project
checkpoint 2° semestre 2026 - engenharia de software

Bruno Takaya - 3ECA - 554986
Iury Cardoso Araujo - 3ECA - 558850
Kethely Ester da Silva - 3ECA - 559187
Raissa Yukari Senoi - 3ECR - 558120
Vanessa Iris Nobre Ribas - 3ECA - 559211

# 📦 Sistema de Controle de Inventário e Gestão de Depósitos

## 🎯 Sobre o Projeto

O **SPI (Sistema de Planejamento e Inventário)** é uma solução de software projetada para automatizar e otimizar a gestão de depósitos. O objetivo principal é garantir precisão e eficiência no controle de entrada, saída, rastreamento de produtos e auditorias de estoque.

## ⚙️ Funcionalidades Principais

* **Controle de Fluxo:** Registro automatizado de entradas e saídas de mercadorias.
* **Rastreamento de Produtos:** Localização visual e sistêmica de itens dentro do depósito.
* **Gestão de Reposição:** Alertas de estoque baixo e automação de pedidos.
* **Auditoria de Estoque:** Contagem cíclica e conferência de inventário.
* **Autenticação Simulada:** Login de usuários para acesso aos painéis operacionais e gerenciais.

## 📂 Estrutura do Projeto

Nossa arquitetura foi pensada para suportar a transição entre o planejamento inicial e a escalabilidade do código.

```text
📦 Front-SPI-2026
 ┣ 📂 docs                  # Requisitos, arquitetura e regras de negócio
 ┣ 📂 public                # Arquivos estáticos (favicon, index.html)
 ┣ 📂 src                   # Código-fonte da aplicação
 ┃ ┣ 📂 assets              # Imagens, logos e CSS global
 ┃ ┣ 📂 components          # Componentes reutilizáveis (Botões, Inputs, Tabelas)
 ┃ ┣ 📂 mocks               # Dados fictícios (JSON/JS) simulando o BD
 ┃ ┣ 📂 pages               # Telas principais (Login, Dashboard, Estoque)
 ┃ ┣ 📂 routes              # Configuração de rotas e navegação
 ┃ ┣ 📂 services            # Integração com os mocks (e futura API real)
 ┃ ┗ 📂 utils               # Funções auxiliares (formatação de data, moeda)
 ┣ 📂 tests                 # Planejamento de validação do sistema
 ┣ 📜 package.json          # Gerenciador de dependências e scripts
 ┗ 📜 README.md             # Apresentação e instruções do projeto

Embora o código ainda não tenha sido escrito, o repositório já está preparado para receber a aplicação Frontend e a documentação técnica:

- **`/docs`**: Contém toda a fase de idealização, fluxos e levantamento de requisitos (Funcionais, Não-funcionais e Regras de Negócio).
- **`/src/pages`**: Organizará as telas principais (Dashboard de Estoque, Tela de Auditoria, Registro de Entradas/Saídas).
- **`/src/components`**: Guardará os elementos visuais reutilizáveis em todo o sistema.
- **`/src/services`**: Concentrará a comunicação com o backend e a validação das lógicas de reposição.
- **`/tests`**: Separado para os scripts de validação de software e testes unitários das regras de negócio.