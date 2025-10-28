# 🚀 Eurofarma Innovation Hub: Plataforma de Gestão de Inovação Corporativa

## Descrição do Projeto

O **Eurofarma Innovation Hub** é uma plataforma digital integrada desenvolvida para fomentar e gerir a inovação corporativa na Eurofarma. O projeto visa engajar os 9.000 colaboradores, otimizar o trabalho do time de inovação (com apenas 5 pessoas) e fornecer visibilidade estratégica consolidada para a alta gestão.

**Dores Resolvidas:**
* **Exclusão Digital:** Cerca de 40% dos colaboradores (operacionais) não possuíam acesso a computadores ou e-mail corporativo. A solução é *mobile-first*, garantindo inclusão digital.
* **Escalabilidade e Sobrecarga:** O time de inovação processava centenas de ideias manualmente, resultando em sobrecarga e caos na triagem.
* **Visibilidade Estratégica:** Falta de *dashboards* consolidados, impossibilitando decisões baseadas em dados concretos sobre o ROI dos programas de inovação.

## Pilares e Funcionalidades Chave

A plataforma é construída sobre três pilares fundamentais para transformar a inovação na Eurofarma:

| Pilar | Funcionalidades | Metas a Atingir |
| :--- | :--- | :--- |
| **Inclusão Digital Universal** | Plataforma *mobile-first* em Flutter, permitindo submissão de ideias por *smartphone* (com opção de anexar áudio/imagem). | Garantir que 100% dos colaboradores tenham acesso à plataforma, reduzindo a exclusão em 80%. |
| **Automação e Escalabilidade** | **Triagem Automática** de ideias por algoritmos, **Rotas de Aprovação Dinâmicas** pré-configuradas e Gestão de Feedback Automatizada. | Permitir que 5 pessoas gerenciem ideias de 9.000 colaboradores. Redução de 50% no esforço manual do time de inovação. |
| **Inteligência Estratégica** | *Dashboards* **Power BI** integrados, exibindo métricas como ROI por Projeto, *Heatmap* de Inovação e *Pipeline* de Ideias. | Fornecer *Dashboard* unificado para C-level. Melhorar a tomada de decisão em 20%. |
| **Gamificação e Cultura** | **Sistema de Pontos e *Badges***, *Leaderboards* de Inovações, Trilhas de Aprendizagem e Recompensas Tangíveis. | Engajar 40% dos colaboradores no primeiro ano. |

## Arquitetura e Tecnologia

A arquitetura geral da solução é modular, utilizando uma abordagem **Serverless** para maior agilidade, e foi estruturada sob o *framework* **TOGAF**.

| Camada | Tecnologia | Detalhes e Justificativa |
| :--- | :--- | :--- |
| **Frontend** | **Flutter / Dart** | *Framework* multiplataforma que permite desenvolver para **Mobile, Web e Desktop** a partir de uma única base de código. |
| **Backend** | **Firebase Functions (Node.js)** | Lógica de negócio e automações (*Serverless*), como o cálculo de pontuação e notificações automáticas aos avaliadores. |
| **Banco de Dados** | **Firebase Firestore** | Banco de dados NoSQL em nuvem, otimizado para desempenho e escalabilidade. |
| **Business Intelligence** | **Power BI** | Utilizado para *Dashboards* executivos, consumindo dados do Firestore (ou Oracle SQL, no plano inicial) via conectores e APIs para relatórios em tempo real. |
| **Infraestrutura** | **Firebase Hosting / Cloud Storage** | Hospedagem da aplicação e gestão de arquivos de mídia (imagens/áudios das propostas). |
| **Controle de Versão** | **Git / GitHub** | Versionamento de código e fluxo de colaboração (link do projeto disponível no GitHub). |

## Metodologia e Cronograma

O projeto seguiu a metodologia **Agile com *framework* Scrum**, adaptado para 4 *sprints* principais (3-4 semanas de duração cada).

| Fase | Período (2025) | Foco Principal | Resultados da Sprint |
| :--- | :--- | :--- | :--- |
| **Sprint 1** | Maio | *Discovery* e Planejamento | Requisitos, Protótipos *low-fidelity* (Figma) e Arquitetura preliminar definida. |
| **Sprint 2** | Junho | Desenvolvimento do *Backend* | *Cloud Functions* (automação), Banco de Dados configurado e Testes automatizados (80% de cobertura). |
| **Sprint 3** | Julho–Agosto | *Frontend* e Integração | Aplicação Flutter responsiva, sistema de gamificação e conectores Power BI implementados. |
| **Sprint 4** | Setembro–Outubro | Testes, Refinamento e Implantação | UAT, Testes de Carga (simulando 9.000 usuários), Implantação em produção e Treinamento. |

## Lições Aprendidas

### Pontos Positivos
* **Escolha Tecnológica Acertada:** O uso do **Flutter** resultou em uma **redução de 40% no tempo de desenvolvimento** e garantiu consistência total de UX, simplificando a manutenção.
* **Foco em Performance:** A realização de testes de carga desde as primeiras *sprints* permitiu otimizações incrementais, preparando o sistema para o crescimento orgânico.
* **Gamificação:** A introdução do sistema de pontos e *leaderboards* provou ser um recurso chave para aumentar o engajamento dos usuários.

### Oportunidades de Melhoria
* **Gerenciamento de Dados:** Separar dados da interface, evitando o uso de dados estáticos (*mockados*) e buscando e gerenciando dados dinamicamente do *backend* (**Firestore**).
* **Gerenciamento de Estado:** Para aplicações maiores, considerar soluções mais robustas como *Provider*, *Riverpod* ou *BLoC*, em vez de apenas `StatefulWidget` e `setState`.
* **Qualidade e Robustez:** Implementar testes mais abrangentes (*unitários* e de *integração*) e mecanismos robustos para lidar com erros (falhas de rede, dados inválidos).

## Roadmap de Evolução (Pós-Lançamento)

| Fase | Período Estimado | Foco | Exemplos de Funcionalidades |
| :--- | :--- | :--- | :--- |
| **Fase 1** | Próximos 6 meses | Inteligência e Expansão | Implementação de IA (NLP para análise de ideias, Chatbot) e Expansão para unidades internacionais e parceiros. |
| **Fase 2** | 6-12 meses | Inovação e *Intraempreendedorismo* | Marketplace interno de inovações, Programa de *Intraempreendedorismo* e *Blockchain* para proteção de propriedade intelectual. |
| **Fase 3** | 12-24 meses | Maturidade e Liderança | Plataforma como serviço (*PaaS*), Centro de excelência e Certificação ISO 56002 (Gestão da Inovação). |

## Contato e Desenvolvimento

Este projeto foi desenvolvido pela equipe **Eurofarma Innovation Hub** para o **Enterprise Challenge FIAP / Eurofarma**.

**Link do Projeto (GitHub):** [https://github.com/bailooon/eurofarma](https://github.com/bailooon/eurofarma)

**Equipe:**
* Matheus Bailon - 98656
* Kaique Aleixo - 98627
* Thomas Abner - \[Não informado]
* Henrique Vieira de Oliveira - 558777
* Ygor Carneiro - 88170
