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

* **RF01 — Autenticação e Controle de Acesso:** O sistema deve permitir o login de usuários cadastrados, diferenciando perfis administrativos e clínicos.
* **RF02 — Gestão de Clientes (Tutores):** O sistema deve permitir cadastrar, consultar, editar e listar os tutores responsáveis pelos animais.
* **RF03 — Gestão de Pets:** O sistema deve permitir o cadastro de animais vinculados a um tutor, registrando nome, espécie, raça, porte, idade e histórico clínico.
* **RF04 — Gestão de Funcionários e Veterinários:** O sistema deve manter o registro da equipe da clínica, incluindo cargos e identificação profissional dos médicos veterinários.
* **RF05 — Registro de Atendimentos Clínicos:** O sistema deve permitir abrir e registrar atendimentos vinculando o pet, o tutor e o veterinário responsável, com data, descrição e status.
* **RF06 — Gestão de Serviços:** O sistema deve permitir o cadastro de serviços (consultas clínicas, vacinas, exames, procedimentos) e sua associação a um ou mais atendimentos.
* **RF07 — Controle de Produtos e Estoque:** O sistema deve gerenciar o catálogo de produtos (rações, medicamentos, insumos) e atualizar automaticamente a quantidade em estoque após o consumo ou venda em atendimento.
* **RF08 — Fechamento e Resumo Financeiro:** O sistema deve calcular o valor total do atendimento somando os serviços realizados e os produtos adquiridos pelo cliente.

### 1.2 Requisitos Não Funcionais (RNF)

* **RNF01 — Usabilidade e Consistência Visual:** A interface deve seguir padrões claros de UI/UX, com navegação intuitiva entre recepção, prontuário e estoque.
* **RNF02 — Integridade e Normalização dos Dados:** A estrutura de dados deve respeitar a 3ª Forma Normal (3FN), garantindo integridade referencial entre tutores, pets, atendimentos, serviços e produtos.
* **RNF03 — Segurança e Rastreabilidade:** Todas as operações críticas devem estar associadas a um usuário autenticado no sistema.
* **RNF04 — Desempenho:** As consultas de histórico de atendimentos e disponibilidade de produtos devem responder em tempo hábil para uso em balcão e consultório.
* **RNF05 — Manutenibilidade:** A arquitetura e a documentação devem ser modulares e versionadas em Markdown no GitHub para facilitar evoluções futuras.

### 1.3 Histórias de Usuário (HU)

* **HU01 (Recepcionista):** *"Como atendente da recepção, quero cadastrar rapidamente um novo tutor e seu pet para agilizar a abertura do atendimento clínico."*
* **HU02 (Veterinário):** *"Como médico veterinário, quero registrar os serviços aplicados e observações no atendimento do pet para manter o histórico clínico atualizado."*
* **HU03 (Gestor de Estoque):** *"Como administrador, quero que o estoque seja abatido automaticamente ao vincular produtos a um atendimento para evitar rupturas de itens essenciais."*
* **HU04 (Cliente / Tutor):** *"Como tutor, quero visualizar de forma detalhada os serviços realizados, os produtos adquiridos e o valor total do atendimento do meu pet."*
* **HU05 (Gestor da Clínica):** *"Como gestor, quero consultar o volume de atendimentos e o faturamento consolidado por período e por profissional."*

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
