# Plano de Experimento – Scoping e Planejamento

#### Aluno: João Francisco Carvalho Soares de Oliveira Queiroga

## 1. Identificação básica

### 1.1 Título do experimento
Avaliação comparativa da qualidade, velocidade e abrangência de ferramentas de análise de dependências em projetos de software.

### 1.2 ID / código
EXP-TCC-DEP-001

### 1.3 Versão do documento e histórico de revisão
- v0.1 — Rascunho inicial (23/11/2025): criação das seções 1 e 2.
- v0.2 — Rascunho inicial (24/11/2025): criação das seções 3, 4, 5 e 6.

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
Avaliar, por meio de um experimento controlado, a qualidade, velocidade e abrangência de ferramentas de análise de dependências aplicadas em projetos de software de diferentes linguagens, com foco na precisão das detecções, no desempenho durante a execução e na cobertura fornecida sobre vulnerabilidades e versões.

### 3.2 Objetivos específicos
O1 — Avaliar a precisão das ferramentas na identificação de dependências e vulnerabilidades.
O2 — Medir o desempenho das ferramentas em termos de tempo de execução e uso de recursos.
O3 — Analisar a abrangência das ferramentas em diferentes ecossistemas e níveis de profundidade das dependências.
O4 — Comparar a consistência dos resultados entre ferramentas que analisam os mesmos projetos.

### 3.3 Questões de pesquisa / de negócio
Q1.1 — As ferramentas identificam corretamente as dependências presentes nos projetos?
Q1.2 — Qual é a taxa de falsos positivos e falsos negativos na detecção de vulnerabilidades?
Q1.3 — A precisão varia entre linguagens diferentes (Rust, JavaScript/TypeScript, Python)?

Q2.1 — Quanto tempo cada ferramenta leva para analisar projetos de tamanhos distintos?
Q2.2 — Qual é o consumo médio de CPU durante a análise?
Q2.3 — Qual é o consumo médio de memória RAM durante a análise?

Q3.1 — Quantos ecossistemas cada ferramenta suporta nativamente?
Q3.2 — Qual é a profundidade máxima da análise do grafo de dependências?
Q3.3 — Quantos tipos de vulnerabilidades cada ferramenta consegue identificar?

Q4.1 — As ferramentas apresentam resultados consistentes quando analisam o mesmo projeto?
Q4.2 — Há divergências relevantes nas versões detectadas?
Q4.3 — A variação entre execuções sucessivas da mesma ferramenta é significativa?

### 3.4 Métricas associadas (GQM)

#### Tabela GQM (Objetivo → Perguntas → Métricas)

| Objetivo | Pergunta | Métricas |
|---------|----------|-----------|
| O1 | Q1.1 | M1: Precisão geral, M2: Recall |
| O1 | Q1.2 | M3: Taxa de falsos positivos, M4: Taxa de falsos negativos |
| O1 | Q1.3 | M1: Precisão geral, M5: Precisão por linguagem |
| O2 | Q2.1 | M6: Tempo total de execução, M7: Tempo médio por arquivo |
| O2 | Q2.2 | M8: Uso médio de CPU, M9: Pico de CPU |
| O2 | Q2.3 | M10: Uso médio de RAM, M11: Pico de RAM |
| O3 | Q3.1 | M12: Número de ecossistemas suportados, M13: Número de gerenciadores suportados |
| O3 | Q3.2 | M14: Profundidade da árvore de dependências, M6: Tempo total de execução |
| O3 | Q3.3 | M5: Precisão por linguagem, M3: Taxa de falsos positivos |
| O4 | Q4.1 | M1: Precisão geral, M4: Taxa de falsos negativos |
| O4 | Q4.2 | M15: Divergência de versões entre ferramentas, M16: Divergência de vulnerabilidades |
| O4 | Q4.3 | M17: Variação entre execuções, M6: Tempo total de execução |

---

#### Tabela geral das métricas (descrição e unidade)

| Métrica | Descrição | Unidade |
|--------|-----------|---------|
| M1 — Precisão geral | Proporção de detecções corretas sobre o total esperado | Percentual |
| M2 — Recall | Proporção de dependências esperadas que foram detectadas | Percentual |
| M3 — Taxa de falsos positivos | Itens detectados incorretamente | Percentual |
| M4 — Taxa de falsos negativos | Itens não detectados, mas presentes | Percentual |
| M5 — Precisão por linguagem | Precisão calculada por ecossistema específico | Percentual |
| M6 — Tempo total de execução | Tempo para completar a análise | Segundos |
| M7 — Tempo médio por arquivo | Tempo médio gasto por arquivo processado | Milissegundos |
| M8 — Uso médio de CPU | Média percentual de uso da CPU durante a execução | Percentual |
| M9 — Pico de CPU | Maior uso registrado durante a análise | Percentual |
| M10 — Uso médio de RAM | Quantidade média de memória utilizada | Megabytes |
| M11 — Pico de RAM | Maior uso registrado de memória | Megabytes |
| M12 — Número de ecossistemas suportados | Quantidade de linguagens/ecossistemas analisáveis | Contagem |
| M13 — Número de gerenciadores suportados | Total de gerenciadores de pacotes compatíveis | Contagem |
| M14 — Profundidade da árvore de dependências | Número máximo de níveis analisados | Níveis |
| M15 — Divergência de versões | Diferença de versões detectadas entre ferramentas | Contagem |
| M16 — Divergência de vulnerabilidades | Diferença de vulnerabilidades identificadas entre ferramentas | Contagem |
| M17 — Variação entre execuções | Variação dos resultados em múltiplas execuções | Percentual |


## 4. Escopo e contexto do experimento

### 4.1 Escopo funcional / de processo
O experimento envolve a análise de dependências em projetos open-source utilizando ferramentas de escaneamento automatizado. Estão incluídos: análise de dependências, detecção de vulnerabilidades, coleta de métricas e comparação estatística.
Ficam excluídos: análise manual de código-fonte, testes de caixas pretas, análise de desempenho de runtime, e qualquer funcionalidade de integração contínua.

### 4.2 Contexto do estudo
O estudo ocorre no contexto de um TCC acadêmico e utiliza repositórios públicos hospedados no GitHub e GitLab. O ambiente experimental será configurado em containers para garantir reprodutibilidade. Os projetos analisados serão escritos em Rust, JavaScript/TypeScript e Python.

### 4.3 Premissas
As ferramentas escolhidas funcionam corretamente em seus ambientes padrão.
Os repositórios selecionados representam adequadamente seus ecossistemas.
As bases de vulnerabilidade públicas estão atualizadas no momento da coleta.

### 4.4 Restrições
Tempo limitado para execução e repetição dos experimentos.
Restrição ao uso de ferramentas open-source ou com versões gratuitas.
Dependência da disponibilidade das APIs públicas usadas pelas ferramentas.

### 4.5 Limitações previstas
Resultados podem não generalizar para projetos muito maiores ou ecossistemas fora dos três analisados.
Ferramentas podem sofrer variações de desempenho dependendo da máquina física, mesmo usando containers.
Atualizações das ferramentas após o experimento podem modificar sua precisão e desempenho, afetando comparações futuras.

## 5. Stakeholders e impacto esperado

### 5.1 Stakeholders principais
Os principais stakeholders incluem: estudante responsável pelo TCC, orientador acadêmico, colegas e avaliadores da banca, além de desenvolvedores e equipes que utilizam ferramentas de análise de dependências em ambientes profissionais. Plataformas que fornecem dados de vulnerabilidades (como bases públicas) também são consideradas partes indiretas interessadas.

### 5.2 Interesses e expectativas dos stakeholders
O estudante espera validar o experimento e obter resultados quantitativos que sustentem o TCC. O orientador e a banca esperam rigor metodológico e clareza na análise dos dados. Desenvolvedores e equipes de engenharia esperam identificar quais ferramentas oferecem melhor precisão, desempenho e cobertura. A comunidade técnica pode esperar recomendações práticas que ajudem na escolha de ferramentas de segurança e análise de dependências.

### 5.3 Impactos potenciais no processo / produto
O experimento pode influenciar decisões sobre ferramentas utilizadas em pipelines de desenvolvimento, além de gerar recomendações que afetem qualidade de código, segurança e prazos de entrega. Também pode aumentar a carga de trabalho momentânea devido à coleta e análise das métricas, mas tende a reduzir retrabalho a longo prazo ao orientar escolhas mais adequadas.

## 6. Riscos de alto nível, premissas e critérios de sucesso

### 6.1 Riscos de alto nível
Os principais riscos envolvem falhas das ferramentas durante a execução, incompatibilidades entre versões ou ecossistemas, instabilidade das APIs públicas e indisponibilidade de repositórios selecionados. Há risco metodológico caso as métricas não sejam coletadas de forma consistente, bem como risco de viés na escolha dos projetos analisados. Restrições de tempo também podem comprometer a repetição necessária das execuções.

### 6.2 Critérios de sucesso globais
O experimento é considerado bem-sucedido se todas as ferramentas selecionadas forem executadas de forma reproduzível, se todas as métricas forem coletadas corretamente e se os resultados permitirem comparar de maneira clara precisão, desempenho e abrangência. É necessário também que os dados obtidos permitam responder todas as questões definidas no GQM e contribuam para as conclusões do TCC.

### 6.3 Critérios de parada antecipada
O experimento deve ser suspenso se alguma ferramenta apresentar falhas críticas que impeçam a coleta de dados, se APIs públicas essenciais estiverem indisponíveis por tempo prolongado ou se os repositórios selecionados não puderem ser analisados adequadamente. O experimento também deve ser interrompido se não houver tempo suficiente para executar todas as repetições previstas e garantir validade estatística mínima.


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
