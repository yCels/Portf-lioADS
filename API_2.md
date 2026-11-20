# API 2 - DeepCode

<p align="center">
  <strong>2º Semestre • 2025-1</strong><br>
  IDE desktop integrada a uma Inteligência Artificial local<br>
  Papel exercido no Scrum: <strong>Scrum Master</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Tipo-Desktop-informational?style=for-the-badge" alt="Aplicação desktop">
  <img src="https://img.shields.io/badge/Papel-Scrum%20Master-orange?style=for-the-badge" alt="Scrum Master">
  <img src="https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge" alt="Projeto concluído">
</p>

---

<a id="atalhos"></a>

<br>

## 📌 Atalhos

- [Identificação do projeto](#identificacao-do-projeto)
- [🏢 Empresa parceira](#empresa-parceira)
- [❗ Problema](#problema)
- [✅ Solução](#solucao)
- [📅 Cronograma e entregas](#cronograma-e-entregas)
- [🔗 Link do repositório Git](#link-do-repositorio-git)
- [🖥️ Preview da aplicação](#preview-da-aplicacao)
- [🛠️ Tecnologias utilizadas](#tecnologias-utilizadas)
- [👨‍💻 Contribuições pessoais](#contribuicoes-pessoais)
- [🧠 Hard skills](#hard-skills)
- [🤝 Soft skills](#soft-skills)
- [📚 Aprendizados](#aprendizados)

---

<a id="identificacao-do-projeto"></a>

<br>

## Identificação do projeto

| Item | Descrição |
|---|---|
| Semestre do curso | 2º semestre |
| Ano e semestre | 2025-1 |
| Nome do projeto | DeepCode |
| Tipo de sistema | Aplicação desktop (IDE) com IA local |
| Papel no Scrum | Scrum Master |
| Atuação técnica | Interface JavaFX (menu lateral de histórico) e integração com o banco de dados |
| Equipe | DeepCode |
| Metodologia | Scrum, com três sprints, reviews e Feira de Soluções |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Empresa parceira | Fatec São José dos Campos - Prof. Jessen Vidal |
| Contexto | Projeto acadêmico do 2º semestre, baseado na metodologia API (RPBL, validação externa e mentalidade ágil) |

---

<a id="problema"></a>

<br>

## ❗ Problema

Quem está aprendendo a programar, especialmente resolvendo listas de exercícios em Python, perde muito tempo procurando erros no próprio código e nem sempre tem alguém para revisar ou sugerir melhorias. As ferramentas com IA disponíveis costumam ficar fora do ambiente onde o código é escrito, dependem de serviços pagos na nuvem e não guardam o histórico das dúvidas.

O desafio foi desenvolver um **Ambiente Integrado de Desenvolvimento (IDE)** que ajudasse o desenvolvedor a ganhar tempo e reduzir custos, com uma IA capaz de corrigir código, sugerir melhorias e completar trechos, guardando as perguntas e respostas para consulta posterior.

---

<a id="solucao"></a>

<br>

## ✅ Solução

A equipe desenvolveu o **DeepCode**, uma IDE desktop em **Java com JavaFX** integrada a um modelo de linguagem executado localmente pelo **Ollama**. O modelo, baseado no **Qwen 2.5 Coder (3B)**, foi configurado por um `Modelfile` com instruções para detectar, corrigir e apontar erros em códigos Python de exercícios. O usuário escreve o código, envia para a IA com um botão e recebe a resposta em uma área separada do editor.

As perguntas e as sugestões ficam salvas em um banco **MySQL** e aparecem em um menu lateral de histórico, onde o usuário pode reabrir, atualizar ou excluir os registros.

### Principais funcionalidades

- Editor de código Python simples dentro da IDE.
- Envio do código para a IA local com um botão.
- Resposta da IA em uma caixa de texto separada do código.
- Correção, sugestões e recomendações de melhoria geradas pelo modelo.
- Histórico de perguntas e respostas salvo em MySQL (CRUD via DAO).
- Menu lateral (sidebar) para consultar, atualizar e excluir o histórico.
- Executável `.jar`, script de inicialização e tutorial de instalação.

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Período | Principais entregas | Situação |
|---|---|---|---|
| Kick-off | 24/02/2025 a 28/02/2025 | Apresentação do desafio e formação do time | Concluído |
| Sprint 1 | 10/03/2025 a 30/03/2025 | IDE base, integração com a IA, botão de envio e caixa de resposta | Concluída |
| Sprint 2 | 07/04/2025 a 27/04/2025 | Interface mais intuitiva e conexão com o banco de dados (CRUD) | Concluída |
| Sprint 3 | 05/05/2025 a 25/05/2025 | Histórico no banco, menu lateral de consulta e tutorial de instalação | Concluída |
| Feira de Soluções | 29/05/2025 | Apresentação do projeto | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Repositório do DeepCode](https://github.com/API-DeepCode/API2)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Tutorial de instalação e execução da IDE](https://www.youtube.com/watch?v=vB7EBUyKuwA)

O repositório também traz o MVP, os backlogs das sprints, os gráficos de burndown e o modelo lógico do banco na pasta de documentação.

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" width="48" height="48" alt="Java" title="Java">
  &nbsp;
  <img src="https://cdn.simpleicons.org/ollama/000000" width="48" height="48" alt="Ollama" title="Ollama">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mysql/mysql-original.svg" width="48" height="48" alt="MySQL" title="MySQL">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/css3/css3-original.svg" width="48" height="48" alt="CSS3" title="CSS (JavaFX)">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/eclipse/eclipse-original.svg" width="48" height="48" alt="Eclipse" title="Eclipse">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" width="48" height="48" alt="Git" title="Git">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/github/github-original.svg" width="48" height="48" alt="GitHub" title="GitHub">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Interface desktop | Java e JavaFX (com CSS) | Editor, botões, caixa de resposta e menu lateral de histórico |
| Inteligência Artificial | Ollama e Qwen 2.5 Coder 3B (Modelfile) | Correção e sugestões de melhoria de código Python, rodando localmente |
| Integração com a IA | HttpURLConnection e org.json | Requisição HTTP para a API local do Ollama e leitura da resposta em JSON |
| Banco de dados | MySQL e JDBC | Persistência do histórico de perguntas e respostas |
| Arquitetura | Padrão DAO e ConnectionFactory | Separação entre interface, acesso a dados e modelo |
| Ambiente e colaboração | Eclipse, IntelliJ, Git e GitHub | Desenvolvimento, branches por integrante e pull requests |
| Metodologia | Scrum | Backlog do produto, backlogs das sprints e burndown |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **Scrum Master** da equipe. Organizei as cerimônias do Scrum, acompanhei o andamento das tarefas de cada integrante e ajudei a remover impedimentos, principalmente na integração das branches individuais com a `main`. Também revisei e aprovei a maior parte dos pull requests do time, como os das branches `Fabio`, `Luiz`, `gustavo`, `josue` e `nícolas`, e mantive o README do repositório atualizado com o cronograma e a situação de cada sprint.

Na parte técnica, na Sprint 3, desenvolvi o **menu lateral de histórico** da IDE. Reorganizei a estrutura do projeto (pasta `Interfacep`) e implementei em JavaFX a sidebar que lista as consultas salvas, integrando-a ao `HistoricoDAO` e ao banco MySQL. Em conjunto com o colega Pedro, adicionei os botões de **atualizar** e **excluir** registros do histórico, com os métodos correspondentes no DAO e os estilos no CSS da aplicação.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Java | Sei fazer com autonomia | Implementação do menu lateral e dos eventos dos botões |
| JavaFX e CSS | Sei fazer com autonomia | Construção e estilização da sidebar de histórico |
| MySQL e JDBC | Sei fazer com autonomia | Consultas, atualização e exclusão de registros do histórico |
| Padrão DAO | Sei fazer com autonomia | Novos métodos no `HistoricoDAO` para atualizar e excluir |
| Ollama e LLM local | Faço com ajuda | Entendimento da integração da IDE com o modelo Qwen via API local |
| Git e GitHub | Sei fazer com autonomia | Revisão e merge de pull requests das branches do time |
| Scrum Master | Sei fazer com autonomia | Condução das cerimônias, acompanhamento do backlog e do cronograma |

</details>

---

<a id="soft-skills"></a>

<br>

## 🤝 Soft skills

<details>
  <summary><strong>Clique para visualizar as soft skills desenvolvidas no projeto</strong></summary>

<br>

| Soft skill | Exemplo pontual no projeto |
|---|---|
| Liderança | Como Scrum Master, conduzi as reuniões e mantive o time focado nas user stories priorizadas para cada sprint |
| Organização | Atualizei o cronograma e o status das sprints no README e acompanhei os burndowns ao longo do semestre |
| Comunicação | Fiz a ponte entre os integrantes que trabalhavam na IA, no banco e na interface para que as partes se encaixassem |
| Resolução de problemas | Coordenei os merges das várias branches individuais com a `main`, resolvendo conflitos antes das entregas |
| Colaboração | Desenvolvi os botões de atualizar e excluir em parceria com outro integrante, dividindo o trabalho entre interface e DAO |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

Ser Scrum Master me ensinou que boa parte do sucesso de um projeto vem da organização: deixar claro quem faz o quê, acompanhar prazos e integrar o trabalho de todos com frequência. Ver várias branches individuais sendo juntadas no fim de cada sprint me mostrou o valor de integrar cedo e com frequência.

Tecnicamente, foi meu primeiro projeto desktop e meu primeiro contato com **IA executada localmente**. Entendi como uma aplicação conversa com um modelo de linguagem por HTTP e como um `Modelfile` define o comportamento do modelo. Também aprofundei Java, JavaFX e o padrão DAO para separar interface e acesso a dados, uma base que usei depois nos projetos de backend.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 1 • Horus](./API_1.md) | [➡️ API 3 • EntreNova Flix](./API_3.md) |

</div>
