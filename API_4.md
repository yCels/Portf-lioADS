# API 4 - Blueprint

<p align="center">
  <strong>4º Semestre • 2026-1</strong><br>
  Geração automatizada de documentos técnicos de engenharia a partir de plantas CAD<br>
  Papel exercido no Scrum: <strong>Desenvolvedor</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Projeto%20Acad%C3%AAmico-Fatec%20SJC-blue?style=for-the-badge" alt="Projeto Acadêmico Fatec SJC">
  <img src="https://img.shields.io/badge/Sistema-Web%20%2B%20IA-informational?style=for-the-badge" alt="Sistema web com IA">
  <img src="https://img.shields.io/badge/Papel-Desenvolvedor-orange?style=for-the-badge" alt="Desenvolvedor">
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
| Semestre do curso | 4º semestre |
| Ano e semestre | 2026-1 |
| Nome do projeto | Blueprint |
| Tipo de sistema | Aplicação web com pipeline de IA para engenharia civil |
| Papel no Scrum | Desenvolvedor |
| Atuação técnica | Backend (Django REST) e pipeline de IA: extração DXF, orçamento e memorial descritivo |
| Equipe | Equipe SUL |
| Metodologia | Scrum, com três sprints, DoR, DoD e Jira |

---

<a id="empresa-parceira"></a>

<br>

## 🏢 Empresa parceira

| Item | Descrição |
|---|---|
| Demanda | Exército Brasileiro |
| Contexto do desafio | Elaboração de documentação técnica de obras (memoriais, especificações e orçamentos) para licenciamento e licitação |
| Parceiro acadêmico | Fatec São José dos Campos - Prof. Jessen Vidal |

---

<a id="problema"></a>

<br>

## ❗ Problema

Para licenciar uma obra, o Exército Brasileiro precisa produzir documentos técnicos detalhados, como **memoriais de cálculo**, **especificações** e **orçamentos**, seguindo as normas da ABNT e padrões internos. Esses documentos servem de base para o processo formal de **licitação**.

Hoje esse trabalho é feito manualmente pelos engenheiros, desde a interpretação dos arquivos CAD até a formatação final dos documentos. O processo consome muitas horas de profissionais especializados, está sujeito a erros de levantamento e atrasa a aprovação das obras.

---

<a id="solucao"></a>

<br>

## ✅ Solução

Desenvolvemos o **Blueprint**, uma aplicação web em que o engenheiro cadastra a obra, envia os arquivos do projeto (plantas **DXF**, CSV ou Excel) e recebe os documentos técnicos padronizados. Um pipeline em Python extrai e calcula os quantitativos da planta de forma determinística. Em seguida, a IA, com **RAG** sobre a base **SINAPI** e as normas NBR, relaciona os itens extraídos aos insumos oficiais, gera o **orçamento** e redige o **memorial descritivo**, exportado em PDF.

### Principais funcionalidades

- Cadastro, edição e listagem de obras pelo engenheiro, com login e cadastro de usuários.
- Upload de arquivos da obra (DXF, CSV ou Excel) e validação da estrutura.
- Motor CAD: leitura do DXF, reconstrução de polígonos, identificação de cômodos e cálculo de áreas e perímetros.
- Mapeamento "De-Para" dos nomes do CAD para a base oficial, com revisão e margem de perda por item.
- Cadastro dos itens do projeto extraídos pela IA e adição manual de itens faltantes.
- Correspondência com a tabela **SINAPI** (palavra-chave + LLM) e cálculo do orçamento, exportado em `.xlsx`.
- Geração do **memorial descritivo** com LangGraph e exportação em PDF, com pré-visualização no frontend.

### Organização da solução

| Componente | Responsabilidade |
|---|---|
| Blueprint (repositório principal) | Documentação, backlog, sprints e submódulos do frontend e do backend |
| blueprint-backend | API Django REST, banco PostgreSQL e módulo de IA (CAD Engine, RAG, LangGraph, orçamento e PDF) |
| blueprint-frontend | Interface React + TypeScript para obras, uploads, revisão e visualização dos documentos |

---

<a id="cronograma-e-entregas"></a>

<br>

## 📅 Cronograma e entregas

| Etapa | Período | Principais entregas | Situação |
|---|---|---|---|
| Sprint 1 | 16/03/2026 a 05/04/2026 | Upload e validação de arquivos, mapeamento De-Para, revisão de itens, dashboard e cadastro de obras | Concluída |
| Sprint 2 | 13/04/2026 a 03/05/2026 | Contexto para a IA, confirmação com a SINAPI, cálculo de quantitativos e exportação do memorial | Concluída |
| Sprint 3 | 11/05/2026 a 31/05/2026 | Login e cadastro, pré-visualização de documentos, edição de obras, memorial estruturado e orçamento correto | Concluída |

---

<a id="link-do-repositorio-git"></a>

<br>

## 🔗 Link do repositório Git

- [Blueprint — repositório principal](https://github.com/Equipe-SUL/Blueprint)
- [Blueprint Backend](https://github.com/Equipe-SUL/blueprint-backend)
- [Blueprint Frontend](https://github.com/Equipe-SUL/blueprint-frontend)

---

<a id="preview-da-aplicacao"></a>

<br>

## 🖥️ Preview da aplicação

[▶️ Assistir à demonstração do produto final](https://www.youtube.com/watch?v=aQZifRPN6wY)

---

<a id="tecnologias-utilizadas"></a>

<br>

## 🛠️ Tecnologias utilizadas

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg" width="48" height="48" alt="Python" title="Python">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/django/django-plain.svg" width="48" height="48" alt="Django" title="Django">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg" width="48" height="48" alt="PostgreSQL" title="PostgreSQL">
  &nbsp;
  <img src="https://cdn.simpleicons.org/ollama/000000" width="48" height="48" alt="Ollama" title="Ollama">
  &nbsp;
  <img src="https://cdn.simpleicons.org/langchain/1C3C3C" width="48" height="48" alt="LangChain e LangGraph" title="LangChain e LangGraph">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg" width="48" height="48" alt="React" title="React">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="48" height="48" alt="TypeScript" title="TypeScript">
  &nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/jira/jira-original.svg" width="48" height="48" alt="Jira" title="Jira">
</p>

| Área | Tecnologias | Aplicação no projeto |
|---|---|---|
| Backend | Python, Django e Django REST Framework | Models, serializers, views e rotas de obras, arquivos, itens e documentos |
| Autenticação | Simple JWT e bcrypt | Login e cadastro de usuários |
| Banco de dados | PostgreSQL (local ou Supabase) e migrations do Django | Persistência de projetos, arquivos, itens, catálogo e memoriais |
| Processamento CAD | ezdxf, NetworkX e GeoJSON | Leitura do DXF, polígonos, cômodos, áreas, perímetros e topologia |
| Inteligência Artificial | Ollama, LangChain e LangGraph | Grafo de geração do memorial descritivo e correspondência com a SINAPI |
| RAG | ChromaDB e embeddings Hugging Face | Base vetorial com cerca de 4.820 itens SINAPI e normas NBR |
| Documentos | Geração de PDF e exportação `.xlsx` | Memorial descritivo em PDF e orçamento em planilha |
| Frontend | React, TypeScript e Vite | Telas de obras, upload, revisão e visualização dos documentos |
| Gestão e colaboração | Jira, Git e GitHub | Tarefas por requisito (T01, T03, T12...), branches e pull requests |

---

<a id="contribuicoes-pessoais"></a>

<br>

## 👨‍💻 Contribuições pessoais

Atuei como **desenvolvedor backend e de IA** no repositório `blueprint-backend`, com cerca de 16 commits ligados a tarefas do Jira.

Na **Sprint 1**, implementei o **endpoint de listagem de obras** (T03) e modelei o domínio dos itens de projeto: criei o model `ItemProjeto`, com um enum para a origem do item (extraído pela IA ou adicionado manualmente), o serializer, a `ItemProjetoView` em `APIView` com as validações do `POST` e a rota de cadastro dos itens a partir do `id_projeto` depois da extração da IA. Também implementei a tarefa **T12**, de **adição manual de itens faltantes**, criando a tabela de catálogo e as migrations.

Na **Sprint 2**, refatorei os prompts e os módulos de visão e de orquestração da IA e removi scripts de teste obsoletos. Corrigi a `UploadView`, que não salvava o projeto no banco, e implementei o **pipeline completo do upload do DXF até a extração orçamentária**, com extração e cálculo de quantitativos, adaptador para o formato do orçamento e ajustes no RAG e nos models.

Na **Sprint 3**, construí o **grafo de IA com LangGraph** a partir do planejamento do time, com estado, nós e arestas condicionais, além de módulos de classificação de layers e extração do DXF. Depois reestruturei o grafo para o **memorial descritivo** (`grafo_novo`), com prompts próprios, o `descritivo_service` e o **gerador de PDF**, e criei a URL e a view que geram o PDF exibido no modal do frontend.

---

<a id="hard-skills"></a>

<br>

## 🧠 Hard skills

<details>
  <summary><strong>Clique para visualizar as hard skills desenvolvidas no projeto</strong></summary>

<br>

| Hard skill | Nível de proficiência | Evidência no projeto |
|---|---|---|
| Python | Sei fazer com autonomia | Services, pipeline de extração e módulos de IA |
| Django e Django REST Framework | Sei fazer com autonomia | Models, serializers, APIViews, rotas e migrations |
| Modelagem de dados e PostgreSQL | Sei fazer com autonomia | `ItemProjeto` com enum de origem, catálogo de itens e memorial |
| LangGraph e LangChain | Sei fazer com autonomia | Grafo de geração do memorial descritivo (estado, nós e arestas) |
| Engenharia de prompt | Sei fazer com autonomia | Prompts do memorial descritivo e refatoração dos prompts existentes |
| RAG e ChromaDB | Faço com ajuda | Uso da base vetorial SINAPI no pipeline de orçamento |
| Processamento de DXF | Faço com ajuda | Pipeline do upload até a extração de quantitativos |
| Geração de PDF | Sei fazer com autonomia | Gerador do memorial descritivo e endpoint para o frontend |
| Git, GitHub e Jira | Sei fazer com autonomia | Commits vinculados a tarefas, branches e merges entre tarefas |

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
| Resolução de problemas | Identifiquei e corrigi a falha da `UploadView`, que impedia o projeto de ser salvo e travava o restante do pipeline |
| Pensamento analítico | Entendi um domínio novo (CAD, SINAPI e memoriais) para transformar a necessidade dos engenheiros em etapas de pipeline |
| Colaboração | Implementei o grafo de IA seguindo o planejamento definido em conjunto e o integrei ao frontend pelo modal de PDF |
| Organização | Trabalhei por tarefas do Jira (T03, T12...), fazendo merge entre elas quando uma dependia da configuração da outra |
| Adaptabilidade | Reestruturei o grafo quando o foco da Sprint 3 passou a ser a qualidade do memorial descritivo |

</details>

---

<a id="aprendizados"></a>

<br>

## 📚 Aprendizados

O Blueprint foi o projeto tecnicamente mais desafiador até agora. Aprendi a construir uma **API REST com Django REST Framework** e a modelar o domínio com cuidado, e vi que uma decisão simples, como o enum de origem do item, facilita muito o trabalho das etapas seguintes.

O maior aprendizado foi combinar **processamento determinístico** com **IA**. Os quantitativos precisam ser exatos, então vêm do cálculo sobre a planta, enquanto a IA entra para relacionar os itens à SINAPI e redigir o memorial. Trabalhar com **LangGraph** me ensinou a dividir uma tarefa de IA em etapas com estado, o que torna o resultado mais controlável e fácil de depurar.

Também aprendi a importância de entender o domínio do cliente. Sem compreender o que é um memorial descritivo e como funciona uma licitação, não seria possível gerar documentos úteis para os engenheiros.

---

<div align="center">

## 🧭 Navegação do portfólio

| 🏠 Página inicial | ⬅️ Projeto anterior | ➡️ Próximo projeto |
|---|---|---|
| [README](./README.md) | [⬅️ API 3 • EntreNova Flix](./API_3.md) | — |

</div>
