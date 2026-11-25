# 🐾 Paraíso Animal — Documentação do Projeto de Engenharia de Software

Documentação consolidada do sistema de gestão clínica e pet shop **Paraíso Animal**, reunindo o planejamento, a especificação de requisitos, a modelagem comportamental e estrutural (UML), os padrões de arquitetura e os protótipos de interface.

---

## 👥 Equipe

* **Wilton Rezende**
* **Kamila Dias**
* **Lucas Santana**
* **Vitória Rocha**

---

## 🔗 Central de Acesso Rápido (Artefatos do Projeto)

| Artefato | Ferramenta | Link de Acesso |
| :--- | :--- | :--- |
| **Quadro de Planejamento e Tarefas** | Trello | [Acessar Quadro Paraíso Animal](https://trello.com/b/BXPyITFK/paraiso-animal-system) |
| **Diagramas UML (Casos de Uso, Sequência, Atividades e Classes)** | Draw.io | [Abrir Arquivo de Modelagem UML](https://app.diagrams.net/#G1fEzNhCUGIa7npEyY7ePCgr8QMZxFeTl1#%7B%22pageId%22%3A%22bFnKCDMHGTz6iA1lRIzV%22%7D) |
| **Protótipo Interativo do Site (Navegável)** | Figma Make | [Testar Protótipo Interativo (Tela Cheia)](https://www.figma.com/make/MkVmEB6tkQDbBd5SVnTWwu/Prot%C3%B3tipo-de-Pet-Shop-Veterin%C3%A1rio?p=f&t=PySglx3xs04KhqgT-0&fullscreen=1) |
| **Mapeamento Completo de Telas (UI/UX)** | Figma Design | [Explorar Telas e Fluxos](https://www.figma.com/design/d0z8b2aExko4s453yqbDBH/Sem-t%C3%ADtulo?node-id=0-1&p=f&t=KHQPkHV1LFy4vqil-0) |

---

## 📋 Gestão e Planejamento (Trello)

O acompanhamento das entregas foi organizado no **Trello**, estruturado por etapas do ciclo de vida do software (*Backlog*, *Em Andamento*, *Revisão* e *Concluído*), garantindo a divisão equilibrada entre levantamento de requisitos, diagramação UML e prototipação das telas.

---

## 📄 Fase 1 — Documento de Especificação de Requisitos (DRS)

### 1.1 Requisitos Funcionais (RF)

* **RF01 — Cadastrar Clientes:** Permitir o cadastro de novos clientes (tutores) no sistema.
* **RF02 — Listar Clientes:** Permitir a consulta e visualização da lista de clientes cadastrados.
* **RF03 — Modificar Clientes:** Permitir a edição e atualização dos dados cadastrais dos clientes.
* **RF04 — Excluir Clientes:** Permitir a exclusão de registros de clientes do sistema.
* **RF05 — Cadastrar Pets:** Permitir o cadastro de pets vinculados aos seus respectivos tutores.
* **RF06 — Listar Pets:** Permitir a consulta e visualização da lista de pets cadastrados.
* **RF07 — Modificar Pets:** Permitir a edição e atualização das informações dos pets.
* **RF08 — Excluir Pets:** Permitir a exclusão de registros de pets do sistema.
* **RF09 — Cadastrar Produtos:** Permitir o cadastro de novos produtos no catálogo do pet shop e clínica.
* **RF10 — Listar Produtos:** Permitir a consulta e visualização dos produtos disponíveis.
* **RF11 — Modificar Produtos:** Permitir a edição e atualização dos dados e estoque dos produtos.
* **RF12 — Excluir Produtos:** Permitir a exclusão de produtos do catálogo.
* **RF13 — Cadastrar Serviços:** Permitir o cadastro de novos serviços oferecidos pela clínica e pet shop.
* **RF14 — Listar Serviços:** Permitir a consulta e visualização dos serviços cadastrados.
* **RF15 — Modificar Serviços:** Permitir a edição e atualização das informações dos serviços.
* **RF16 — Excluir Serviços:** Permitir a exclusão de serviços do sistema.
* **RF17 — Agendar Data Consulta:** Permitir selecionar e registrar a data para o agendamento de consultas.
* **RF18 — Agendar Horário Consulta:** Permitir selecionar e registrar o horário específico da consulta agendada.
* **RF19 — Agendar Confirma Consulta:** Permitir confirmar o agendamento da consulta realizada.
* **RF20 — Funcionários Agendar Horários:** Permitir que os funcionários gerenciem e realizem o agendamento de horários de atendimento.
* **RF21 — Funcionários Vender Serviços:** Permitir que os funcionários registrem a venda de serviços aos clientes.

### 1.2 Requisitos Não Funcionais (RNF)

* **RNF01 — Definir Aparência do Sistema:** Estabelecer a identidade visual, layout, paleta de cores e padrões de interface (UI/UX) do sistema.
* **RNF02 — Definir Linguagem de Programação:** Padronizar as linguagens de programação e tecnologias utilizadas no desenvolvimento da aplicação.
* **RNF03 — Definir SQL:** Utilizar banco de dados relacional estruturado em SQL para persistência, consultas e integridade das informações.
* **RNF04 — Definir Hospedagem:** Estabelecer a infraestrutura e o ambiente de hospedagem para publicação e disponibilidade do sistema.

### 1.3 Histórias de Usuário (HU)

* **HU01 (Recepcionista):** *"Como atendente da recepção, quero cadastrar, listar e atualizar tutores e seus pets para manter o registro da clínica sempre organizado."*
* **HU02 (Cliente / Tutor):** *"Como tutor, quero escolher a data, o horário e confirmar a consulta do meu pet para garantir o atendimento."*
* **HU03 (Funcionário):** *"Como funcionário, quero agendar horários e registrar a venda de serviços para agilizar o atendimento no balcão."*
* **HU04 (Gestor / Administrador):** *"Como administrador, quero cadastrar, atualizar e gerenciar o catálogo de produtos e serviços oferecidos pelo pet shop."*

---

## 🔄 Fase 2 — Modelagem Dinâmica (Comportamento)

Os diagramas comportamentais estão centralizados no arquivo oficial do projeto no **Draw.io**, organizados por abas internas:

* **Diagrama de Casos de Uso:** Mapeia as interações dos atores (*Administrador*, *Recepcionista*, *Veterinário*) com as funcionalidades centrais de cadastro, atendimento e controle de estoque.
* **Diagrama de Sequência:** Detalha a troca de mensagens e validações em ordem cronológica durante o fluxo principal de agendamento, execução do atendimento clínico e baixa de produtos.
* **Diagrama de Atividades:** Representa o fluxo operacional completo desde a chegada do tutor com o pet na clínica até o encerramento financeiro do atendimento.

---

## 🏗️ Fase 3 — Modelagem Estática (Estrutura)

A estrutura estática do sistema está documentada na aba de classes do **Draw.io**:

* **Diagrama de Classes:** Define as classes de domínio (`Usuario`, `Funcionario`, `Cliente`, `Pet`, `Atendimento`, `Servico`, `Produto`), seus atributos, métodos e relacionamentos estruturais (`1:N` entre Tutor e Pets; `N:M` entre Atendimentos, Serviços e Produtos).

---

## 🎨 Fase 4 — Interface (UI/UX) e Arquitetura

### 4.1 Especificação de Arquitetura e Padrões

* **Padrão Arquitetural (MVC / Camadas):** Separação clara entre a camada de Apresentação (interfaces prototipadas), Camada de Negócio (regras de atendimento, cálculo de valores e controle de estoque) e Camada de Persistência (banco de dados relacional).
* **Padrões de Projeto Aplicados:**
  * **Repository / DAO:** Isolamento das operações de acesso e manipulação dos registros de clientes, pets e atendimentos.
  * **DTO (Data Transfer Object):** Padronização do tráfego de dados consolidados (ex.: resumo completo de atendimento com serviços e produtos).
  * **Singleton / Gerenciamento de Sessão:** Controle centralizado de conexão e sessão do usuário autenticado.

### 4.2 Estrutura e Divisão dos Protótipos (Figma)

A prototipação do sistema foi dividida em duas frentes complementares para atender tanto à demonstração funcional quanto ao detalhamento completo das interfaces:

1. **Protótipo Interativo do Site (Figma Make):** Versão navegável em tela cheia que simula a experiência real de uso, permitindo testar a transição entre páginas, menus e fluxos principais diretamente no navegador.
2. **Mapeamento Completo de Telas (Figma Design):** Conjunto detalhado de interfaces e variações de estado (cadastros, listagens, modais de confirmação e feedback visual), dividido em seis módulos funcionais:
   * **Acesso e Autenticação:** Telas de login, recuperação de senha, validação de credenciais e seleção de perfil de acesso.
   * **Dashboard e Visão Geral:** Painel principal com indicadores operacionais da clínica, agenda do dia, alertas de estoque e atalhos rápidos.
   * **Gestão de Clientes e Pets:** Fluxos de consulta, cadastro e edição de tutores, além da ficha completa e histórico clínico de cada animal.
   * **Fluxo de Atendimento Clínico:** Etapas de abertura de atendimento, triagem, registro de consulta veterinária, prescrições e vínculo de procedimentos.
   * **Catálogo de Serviços e Estoque:** Gerenciamento de serviços clínicos, controle de entrada e saída de produtos e monitoramento de itens críticos.
   * **Financeiro e Relatórios:** Fechamento de atendimento com soma automática de serviços e produtos, histórico de pagamentos e relatórios gerenciais.
