# Inventory-project
checkpoint 2° semestre 2026 - engenharia de software

* Bruno Takaya - 3ECA - 554986
* Iury Cardoso Araujo - 3ECA - 558850
* Kethely Ester da Silva - 3ECA - 559187
* Raissa Yukari Senoi - 3ECR - 558120
* Vanessa Iris Nobre Ribas - 3ECA - 559211

# 📦 Sistema de Controle de Inventário e Gestão de Depósitos

## 🎯 Sobre o Projeto

O **SPI (Sistema de Planejamento e Inventário)** é uma solução de software projetada para automatizar o controle de entrada, saída, rastreamento de produtos e auditoria de estoque em depósitos. O objetivo principal do sistema é reduzir erros manuais e dar visibilidade em tempo real sobre a posição e a quantidade do inventário.

O projeto foi pensado para que o funcionário possa responder rapidamente a perguntas críticas da operação diária, como: *"onde está esse produto?"*, *"quantas unidades temos?"*, *"em qual corredor estão armazenadas?"* e *"quanto entrou ou saiu do estoque?"*.

## 🚨 O Problema e a Solução

Atualmente, depósitos com um grande volume de itens armazenados em diferentes corredores sofrem com a falta de um controle centralizado, gerando gargalos operacionais. Este sistema foi desenvolvido para solucionar:
* A dificuldade e a perda de tempo na separação, movimentação e busca de itens nos corredores.
* A divergência constante entre a quantidade registrada e a quantidade física existente.
* O armazenamento desorganizado e as dificuldades em realizar conferências e inventários precisos.

## 👥 Perfis de Usuário

A plataforma atende a diferentes agentes dentro da logística do depósito:
* **Operador de Depósito:** Registra entradas, saídas e movimentações físicas do dia a dia, controlando a localização dos itens por corredor.
* **Gestor de Estoque:** Acompanha o dashboard geral, níveis de estoque, aprova reposições e analisa relatório.
* **Auditor:** Realiza conferências de inventário e consulta o histórico de movimentações.
* **Administrador:** Cadastra usuários, configura os corredores do depósito e define permissões de acesso.

## ⚙️ Funcionalidades Principais

* **Dashboard de Inventário:** Visão geral do depósito, total de caixas, corredores utilizados e alertas de estoque baixo.
* **Gestão de Cadastros:** Cadastro de produtos (com estoque mínimo e unidade de medida) e mapeamento de corredores.
* **Movimentações de Estoque:** Registro de entradas e saídas com atualização automática das quantidades e saldos.
* **Rastreamento:** Identificação exata de qual corredor e posição um produto está armazenado.
* **Auditoria de Estoque:** Manutenção de um histórico completo de todas as movimentações (quem fez, o que foi alterado e quando).

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