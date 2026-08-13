# Sistema de Chamados — Portfólio Josy Soares

Sistema de central de atendimento de TI desenvolvido em **Oracle APEX**, **SQL** e **PL/SQL**, criado como projeto de portfólio para demonstrar, na prática, modelagem de dados, regras de negócio, formulários, relatórios e dashboards em um cenário completo de help desk.

> 🎮 **Curiosidade:** para fugir do clichê de "sistema corporativo genérico", os usuários fictícios usados nos testes foram inspirados em personagens do universo Super Mario (Mario, Luigi, Peach, Bowser, Toad, Yoshi, Wario). Projeto independente, sem qualquer vínculo com a Nintendo — feito exclusivamente para fins educacionais e de portfólio.

## Índice

- [Sobre o projeto](#sobre-o-projeto)
- [Como funciona](#como-funciona)
- [Funcionalidades](#funcionalidades)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Capturas de tela](#capturas-de-tela)
- [Testando o sistema](#testando-o-sistema)
- [Autor e contato](#autor-e-contato)

## Sobre o projeto

O sistema simula uma central de atendimento de TI, permitindo:

- Cadastrar usuários (perfil **Usuário** ou **Suporte**);
- Abrir chamados descrevendo um problema ou necessidade;
- Anexar arquivos aos chamados para apoiar a análise;
- Classificar chamados por prioridade e status;
- Acompanhar o atendimento até a resolução;
- Visualizar indicadores em um dashboard.

Todo o fluxo — do cadastro do usuário até o encerramento do chamado — foi construído com regras de negócio reais (validações de campos obrigatórios, triggers, controle de datas de abertura/atendimento/resolução), reproduzindo o dia a dia de um sistema de suporte real.

## Como funciona

| Etapa | Descrição |
|---|---|
| **1. Usuário** | Cadastra-se e abre um chamado descrevendo sua necessidade. |
| **2. Chamado** | Recebe prioridade, status e data de abertura. |
| **3. Suporte** | Um profissional assume o chamado e realiza o atendimento. |
| **4. Anexos** | O usuário pode enviar arquivos para ajudar na análise do problema. |
| **5. Acompanhamento** | O sistema registra os horários e as mudanças do chamado. |
| **6. Resolução** | Após solucionar o problema, o chamado é encerrado. |

## Funcionalidades

| Módulo | Descrição | Recursos |
|---|---|---|
| **Usuários** | Cadastro e gerenciamento de usuários (perfis Usuário/Suporte). | Formulário • Relatório • Tabela • Trigger |
| **Chamados** | Abertura e acompanhamento dos chamados. | Formulário • Relatório • Tabela • Trigger |
| **Suporte** | Gerenciamento dos responsáveis pelos atendimentos. | Formulário • Relatório • Tabela • Trigger |
| **Prioridades** | Controle do nível de urgência dos chamados (Baixa, Média, Alta). | Regra de negócio • Banco de dados |
| **Anexos** | Arquivos relacionados aos chamados. | Upload • BLOB • Oracle Database |
| **Status** | Acompanhamento das etapas do atendimento (Aguardando, Em andamento, Resolvido). | Regra de negócio • Banco de dados |
| **Validações** | Checagem de campos obrigatórios, formatos e regras antes de salvar. | Validation • PL/SQL • Front-end |
| **Dashboard** | Indicadores de chamados por status, prioridade e atendente. | Charts • Relatórios visuais |

### Visões do sistema

O sistema possui páginas separadas por perfil de acesso:

- **Usuários** — cadastro e gerenciamento de usuários.
- **Chamados – Visão do usuário** — o usuário abre e acompanha seus próprios chamados.
- **Chamados – Visão do suporte** — o time de suporte visualiza, assume e trata os chamados abertos (sem opção de criar novos chamados, já que essa ação é exclusiva do usuário solicitante).
- **Dashboard** — indicadores consolidados: total de chamados, chamados sem atendimento, em andamento, resolvidos, distribuição por atendente, por status e por prioridade.

## Tecnologias utilizadas

- **Oracle APEX** — construção das páginas, formulários, relatórios e dashboard.
- **SQL** — modelagem e consultas ao banco de dados.
- **PL/SQL** — regras de negócio, triggers e validações.
- **Oracle Database** — armazenamento de dados, incluindo anexos em BLOB.
- **HTML / CSS** — customização visual da tela inicial (estilização com apoio de IA).

## Capturas de tela

### Tela de login
![Tela de login](screenshots/01-login.png)

### Página inicial do portfólio
![Página inicial](screenshots/02-home-portfolio.png)

### Página inicial integrada ao sistema
![Home integrada ao APEX](screenshots/03-home-embutido-apex.png)

### Relatório de usuários
![Relatório de usuários](screenshots/04-relatorio-usuarios.png)

### Cadastro de novo usuário
![Cadastro de usuário](screenshots/05-cadastro-usuario.png)

### Chamados — visão do usuário
![Chamados visão do usuário](screenshots/06-chamados-visao-usuario.png)

### Abertura de novo chamado
![Abertura de chamado](screenshots/07-abertura-chamado.png)

### Chamados — visão do suporte
![Chamados visão do suporte](screenshots/10-chamados-suporte-ajustado.png)

### Edição de chamado pelo suporte
![Edição de chamado pelo suporte](screenshots/09-edicao-chamado-suporte.png)

### Dashboard
![Dashboard](screenshots/11-dashboard.png)

## Testando o sistema

Fique à vontade para testar o sistema: você pode criar usuários, abrir chamados, cadastrar suportes e ver todo o fluxo funcionando na prática.

🔗 Acesse: `https://oracleapex.com/ords/r/portfolioapex/sistema-de-chamado/home`

> Ambiente de portfólio/demonstração — os dados podem ser reiniciados periodicamente.

## Autor e contato

Desenvolvido por **Josy Soares** (modelagem, banco de dados e PL/SQL) — estilização (CSS) com apoio de IA.

Críticas, dicas e sugestões são muito bem-vindas! Me chama:

- 💼 [LinkedIn](https://www.linkedin.com/in/josysoares/)
- 💬 [WhatsApp](https://wa.me/5511917467228)
