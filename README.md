🏥 Sistema Inteligente de Gestão de Leitos Hospitalares
Status do Projeto: Concluído / Em Portfólio 🚀
📝 Visão Geral
Este projeto nasceu da necessidade de otimizar a rotatividade de leitos em ambientes hospitalares de alta complexidade. O objetivo principal foi reduzir o tempo de ociosidade dos leitos, integrando dados de Manutenção, Limpeza e Enfermagem para evitar perdas financeiras e melhorar o atendimento ao paciente.
⚠️ O Problema de Negócio
Gargalos identificados no fluxo operacional:
Ociosidade "Invisível": Leitos vazios que não constavam como disponíveis por falta de atualização no sistema.
Bloqueios Prolongados: Leitos retidos na manutenção por tempo superior ao necessário.
Falta de Higienização: Atraso na liberação para novos pacientes por falta de integração com a equipe de limpeza.
🛠️ Arquitetura e Tech Stack
O projeto foi estruturado em três pilares principais:
Engenharia de Dados (Python):
Simulação de bases robustas (Excel/CSV) com dados de pacientes, leitos e movimentações.
Limpeza de inconsistências (datas de saída retroativas, IDs duplicados) via Pandas.
Modelagem e ETL (Power BI/Power Query):
Criação da tabela fato Eventos_Movimentacao.
Relacionamentos em esquema Estrela (Star Schema) para performance.
Visualização (Power BI):
Criação de dashboards interativos focados em Storytelling.
📊 Indicadores Chave (KPIs)
No dashboard, foquei no acompanhamento de:
Taxa de Ocupação: Percentual de leitos em uso vs. capacidade total.
Giro de Leito: Tempo médio de permanência do paciente.
Intervalo de Substituição: Tempo entre a saída de um paciente e a entrada de outro (incluindo limpeza).
Impacto Financeiro: Estimativa de perda por leitos bloqueados em manutenção.
🚀 Como Visualizar o Projeto
Devido a restrições de licença do Power BI Service, a interação direta foi substituída por documentação visual:
Clique aqui para baixar o Relatório em PDF
Ver Vídeo de Demonstração (GIF)
