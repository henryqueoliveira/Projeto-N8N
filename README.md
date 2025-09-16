# 🚀 #Projeto N8N: Desvendando a Automação Inteligente no Protheus

Este repositório é o centro técnico da minha jornada de desenvolvimento e descoberta, **#Projeto N8N**. Aqui, estou explorando e construindo soluções para conectar o **TOTVS Protheus** ao poder da automação low-code do **n8n**, visando otimizar processos de negócio de forma inovadora e eficiente.

---

## 🎯 Objetivo do Projeto

O objetivo principal desta jornada é demonstrar e implementar automações de alto impacto, utilizando a flexibilidade das APIs REST do Protheus e a capacidade de orquestração visual do n8n. A meta é ir além das integrações básicas, criando fluxos de trabalho que transformem o Protheus de um sistema de registro passivo em um sistema de ação proativo.

---

## ✅ Status Atual: Marco 1 - Primeira versão da API pronta!

**A primeira versão (v1.0) da API de automação de Notas Fiscais está finalizada e o código-fonte ADVPL já está disponível neste repositório!**

Este não é mais um teste de conceito; é o coração da nossa automação. A API é responsável por:

- **Receber** uma requisição para faturar um Pedido de Venda específico.
- **Orquestrar** internamente a geração do Documento de Saída no Protheus.


A comunicação com o n8n foi um sucesso, validando que o "cérebro" (Protheus) e o "maestro" (n8n) da nossa automação conseguem conversar perfeitamente para executar a tarefa mais crítica do processo.

---

## 🛠️ Tecnologias Envolvidas

* **TOTVS Protheus:** O ERP base para as automações.
* **ADVPL / TL++:** Linguagem de desenvolvimento para APIs e lógicas customizadas no Protheus.
* **SQL Server:** Banco de dados para interação direta quando necessário.
* **n8n:** Plataforma de automação de fluxo de trabalho (iPaaS / low-code).
* **API REST:** Protocolo de comunicação entre sistemas.
* **Node.js:** Ambiente de execução para o n8n localmente.

---

## 🗺️ Próximos Passos: Construindo o Maestro da Automação (Workflow n8n)

Com a API pronta e funcional, o foco agora é 100% no desenvolvimento do fluxo de orquestração ponta-a-ponta no **n8n**. O plano de desenvolvimento para o workflow inclui:

-   **[ ] Gatilho Inteligente:** Criar um agendador que busca periodicamente no Protheus por Pedidos de Venda que estão liberados e prontos para faturar.
-   **[ ] Chamada da API:** Para cada pedido encontrado, acionar a API de faturamento que acabamos de desenvolver.
-   **[ ] Loop de Polling Assíncrono:** Implementar a lógica para consultar o status da NF-e, aguardando a resposta de "Autorizada" ou "Rejeitada".
-   **[ ] Tratamento de Sucesso e Falha:**
    -   Se **autorizada**, prosseguir para a próxima etapa.
    -   Se **rejeitada**, capturar o motivo do erro e notificar a equipe responsável.
-   **[ ] Distribuição Final:** Após a autorização, usar a API do TSS para obter o XML e o DANFE, e então enviar os arquivos por e-mail para o cliente.

O desafio agora é construir um fluxo robusto, resiliente e que lide com todas as variáveis do mundo real.

---

## 🤝 Como Contribuir e Acompanhar

Esta é uma jornada de aprendizado e colaboração! Suas ideias e feedback são muito bem-vindos.

* **Acompanhe no LinkedIn:** Siga a série de posts **#JornadaProtheusN8N** no meu perfil para atualizações semanais, desafios e insights.
* **Sugestões e Ideias:** Sinta-se à vontade para abrir uma [Issue](https://github.com/henryqueoliveira/Projeto-N8N/issues) neste repositório ou comentar nos posts do LinkedIn com suas sugestões para automações ou soluções para os desafios que surgirem.
* **Compartilhe:** Se você achou esta iniciativa interessante, compartilhe com sua rede!

---

## 🔗 Meus Outros Projetos e Perfil

* [Perfil no GitHub](https://github.com/henryqueoliveira)
* [Perfil no LinkedIn](https://www.linkedin.com/in/henryque-marques-de-oliveira)
