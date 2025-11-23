# Plano de Experimento – Scoping e Planejamento

#### Aluno: João Francisco Carvalho Soares de Oliveira Queiroga

## 1. Identificação básica

### 1.1 Título do experimento
Avaliação comparativa da qualidade, velocidade e abrangência de ferramentas de análise de dependências em projetos de software.

### 1.2 ID / código
EXP-TCC-DEP-001

### 1.3 Versão do documento e histórico de revisão
- v0.1 — Rascunho inicial (2025-11-23): criação das seções 1 e 2.

### 1.4 Datas (criação, última atualização)
Data de criação: 23 de novembro de 2025.
Última atualização: 23 de novembro de 2025.

### 1.5 Autores (nome, área, contato)
João Francisco Carvalho Soares de Oliveira Queiroga — Engenharia de Software — joao.queiroga@example.com

### 1.6 Responsável principal (PI / dono do experimento)
João Francisco Carvalho Soares de Oliveira Queiroga — estudante (dono do experimento / responsável técnico)

### 1.7 Projeto / produto / iniciativa relacionada
Projeto de TCC: *DepMonitor* — ferramenta para análise de dependências e identificação de versões e vulnerabilidades em projetos multi-linguagem.

## 2. Contexto e problema

### 2.1 Descrição do problema / oportunidade
Ferramentas de análise de dependências, como scanners de vulnerabilidade e analisadores de grafo, são amplamente utilizadas para detectar versões, vulnerabilidades e relações entre pacotes. Porém, ainda há incertezas quanto à qualidade dos resultados obtidos, ao tempo de execução para analisar projetos de portes variados e ao nível de abrangência em diferentes ecossistemas. O experimento busca comparar ferramentas representativas para apoiar decisões técnicas sobre quais delas oferecem melhor precisão, desempenho e cobertura.

### 2.2 Contexto organizacional e técnico
O experimento é desenvolvido no contexto de um Trabalho de Conclusão de Curso (TCC), com orientação acadêmica e uso de repositórios open-source como base de análise.
No aspecto técnico, os testes envolvem repositórios hospedados em plataformas como GitHub e GitLab, incluindo projetos escritos em Rust, JavaScript/TypeScript e Python. As ferramentas analisadas incluem scanners de dependências e mecanismos de consulta a bases de vulnerabilidade públicas. A execução exige ambientes reprodutíveis por meio de containers e scripts de automação para coleta de métricas de qualidade, desempenho e abrangência.

### 2.3 Trabalhos e evidências prévias
Incluem documentação e relatórios de ferramentas amplamente utilizadas, estudos acadêmicos sobre segurança da cadeia de suprimentos de software e detecção de vulnerabilidades, além de execuções piloto que apoiaram o ajuste preliminar dos procedimentos do experimento.

### 2.4 Referencial teórico e empírico essencial
A fundamentação do experimento envolve conceitos de gerenciamento de dependências, vulnerabilidades e segurança da cadeia de suprimentos de software.
As métricas avaliadas incluem precisão, recall e F1-score para qualidade; tempo de execução e uso de recursos para desempenho; e número de ecossistemas e profundidade da análise para abrangência.
As validações utilizam bases como CVE e NVD, e a comparação estatística dos resultados envolve métodos como t-test, ANOVA ou testes não paramétricos, dependendo da distribuição dos dados.

## 3. Objetivos e questões (Goal / Question / Metric)
### 3.1 Objetivo geral
Preencha o objetivo geral usando um template claro (ex.: GQM).

### 3.2 Objetivos específicos
Decomponha o objetivo geral em metas mais focadas (O1, O2 etc.).

### 3.3 Questões de pesquisa / de negócio
Formule perguntas claras que o experimento responderá.

### 3.4 Métricas associadas (GQM)
Associe métricas às questões, com definição e fonte dos dados.

## 4. Escopo e contexto do experimento
### 4.1 Escopo funcional / de processo
Explique o que será incluído e excluído do experimento.

### 4.2 Contexto do estudo
Caracterize o contexto onde o estudo ocorrerá.

### 4.3 Premissas
Liste as suposições consideradas verdadeiras.

### 4.4 Restrições
Registre limitações práticas (tempo, orçamento, ferramentas, acessos).

### 4.5 Limitações previstas
Explique fatores que podem prejudicar a generalização dos resultados.

## 5. Stakeholders e impacto esperado
### 5.1 Stakeholders principais
Liste os grupos ou papéis impactados pelo experimento.

### 5.2 Interesses e expectativas dos stakeholders
Descreva o que cada grupo espera obter do experimento.

### 5.3 Impactos potenciais no processo / produto
Antecipe como o experimento pode afetar prazos, qualidade ou carga de trabalho.

## 6. Riscos de alto nível, premissas e critérios de sucesso
### 6.1 Riscos de alto nível
Identifique os principais riscos de negócio e técnicos.

### 6.2 Critérios de sucesso globais
Defina as condições para o experimento ser útil e viável.

### 6.3 Critérios de parada antecipada
Descreva situações que exigem adiar ou cancelar o experimento.

## 7. Modelo conceitual e hipóteses
### 7.1 Modelo conceitual do experimento
Explique como os fatores influenciam as respostas.

### 7.2 Hipóteses formais (H0, H1)
Formule hipóteses nulas e alternativas.

### 7.3 Nível de significância e poder
Defina α e discuta poder estatístico.

## 8. Variáveis, fatores, tratamentos e objetos de estudo
### 8.1 Objetos de estudo
Descreva o que será manipulado ou analisado.

### 8.2 Sujeitos / participantes
Caracterize quem serão os participantes.

### 8.3 Variáveis independentes
Liste fatores e níveis.

### 8.4 Tratamentos
Descreva cada condição experimental.

### 8.5 Variáveis dependentes
Informe as medidas de resultado observadas.

### 8.6 Variáveis de controle / bloqueio
Liste fatores que serão mantidos constantes.

### 8.7 Variáveis de confusão conhecidas
Identifique fatores que podem distorcer resultados.

## 9. Desenho experimental
### 9.1 Tipo de desenho
Indique o tipo de desenho experimental e a justificativa.

### 9.2 Randomização e alocação
Explique como será feita a randomização.

### 9.3 Balanceamento e contrabalanço
Descreva como garantir grupos comparáveis.

### 9.4 Número de grupos e sessões
Informe quantos grupos e quantas sessões haverá.

## 10. População, sujeitos e amostragem
### 10.1 População-alvo
Descreva a população real representada no experimento.

### 10.2 Critérios de inclusão
Especifique requisitos mínimos dos participantes.

### 10.3 Critérios de exclusão
Liste condições que impedem participação.

### 10.4 Tamanho da amostra planejado
Defina quantos participantes por grupo.

### 10.5 Método de seleção / recrutamento
Explique como os participantes serão recrutados.

### 10.6 Treinamento e preparação
Descreva materiais ou treinamentos fornecidos.

## 11. Instrumentação e protocolo operacional
### 11.1 Instrumentos de coleta
Liste questionários, logs, formulários, etc.

### 11.2 Materiais de suporte
Descreva instruções, guias ou slides utilizados.

### 11.3 Procedimento experimental
Escreva o passo a passo do experimento.

### 11.4 Plano de piloto
Indique se haverá piloto e critérios de ajuste.

## 12. Plano de análise de dados
### 12.1 Estratégia geral de análise
Explique como os dados responderão às questões.

### 12.2 Métodos estatísticos
Liste testes e técnicas estatísticas.

### 12.3 Tratamento de dados faltantes e outliers
Defina regras prévias para lidar com dados ausentes.

### 12.4 Análise de dados qualitativos
Descreva técnicas para dados qualitativos.

## 13. Avaliação de validade
### 13.1 Validade de conclusão
Liste ameaças e mitigação.

### 13.2 Validade interna
Identifique ameaças e estratégias de controle.

### 13.3 Validade de constructo
Discuta representação dos conceitos medidos.

### 13.4 Validade externa
Discuta generalização dos resultados.

### 13.5 Resumo das ameaças e mitigação
Resuma ameaças principais e ações.

## 14. Ética, privacidade e conformidade
### 14.1 Questões éticas
Descreva questões éticas envolvidas.

### 14.2 Consentimento informado
Explique como será obtido o consentimento.

### 14.3 Privacidade e proteção de dados
Indique que dados serão coletados e como serão protegidos.

### 14.4 Aprovações necessárias
Liste aprovações (comitê de ética, jurídico, etc.).

## 15. Recursos, infraestrutura e orçamento
### 15.1 Recursos humanos e papéis
Identifique membros e seus papéis.

### 15.2 Infraestrutura técnica necessária
Liste ambientes, ferramentas e servidores.

### 15.3 Materiais e insumos
Relacione materiais físicos ou digitais necessários.

### 15.4 Orçamento e custos estimados
Estime custos e fontes de financiamento.

## 16. Cronograma, marcos e riscos operacionais
### 16.1 Macrocronograma
Defina datas e marcos principais.

### 16.2 Dependências entre atividades
Indique dependências entre etapas.

### 16.3 Riscos operacionais e contingência
Liste riscos e estratégias de contingência.

## 17. Governança do experimento
### 17.1 Papéis e responsabilidades formais
Defina responsáveis, executores e revisores.

### 17.2 Ritos de acompanhamento
Descreva reuniões e checkpoints.

### 17.3 Controle de mudanças no plano
Explique processo para registrar mudanças.

## 18. Documentação e reprodutibilidade
### 18.1 Repositórios e convenções
Indique onde documentos e scripts serão armazenados.

### 18.2 Templates e artefatos padrão
Liste modelos utilizados.

### 18.3 Plano de empacotamento
Descreva como facilitar futuras replicações.

## 19. Plano de comunicação
### 19.1 Públicos e mensagens-chave
Liste grupos e mensagens importantes.

### 19.2 Canais e frequência
Defina canais e frequência de comunicação.

### 19.3 Pontos obrigatórios
Especifique eventos que exigem comunicação formal.

## 20. Critérios de prontidão (Definition of Ready)
### 20.1 Checklist de prontidão
Liste itens que devem estar completos antes da execução.

### 20.2 Aprovações finais
Indique quem deve dar o “ok final”.
