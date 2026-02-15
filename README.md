# 🏥 Projeto de Análise de Dados Hospitalares

### Organização, Tratamento e Visualização de Dados de Leitos

---

## 📌 Visão Geral

Este projeto tem como objetivo analisar, organizar e visualizar dados relacionados ao controle de leitos hospitalares, com foco em identificar gargalos operacionais, reduzir processos manuais e melhorar a eficiência na gestão hospitalar.

A solução proposta utiliza análise de dados e visualização interativa para transformar informações operacionais em indicadores estratégicos que auxiliam na tomada de decisão.

---

## 🎯 Objetivos do Projeto

* Monitorar a ocupação e disponibilidade dos leitos em tempo real
* Facilitar o acompanhamento das movimentações de pacientes
* Identificar gargalos operacionais e ineficiências
* Reduzir perdas financeiras causadas por má gestão de leitos
* Criar indicadores estratégicos para apoio à tomada de decisão
* Automatizar análises que antes eram realizadas manualmente

---

## 🚨 Problemas Identificados

Durante o estudo do fluxo hospitalar, foram identificados os seguintes pontos críticos:

* Leitos bloqueados por longos períodos sem justificativa clara
* Reutilização de leitos sem registro adequado de limpeza
* Falta de comunicação entre equipes sobre disponibilidade de leitos
* Leitos disponíveis que não são utilizados por falta de informação
* Falta de integração entre setores como enfermagem, manutenção e administração
* Impacto financeiro causado por baixa eficiência operacional

---

## 🧠 Entendimento do Processo de Negócio

Antes da análise técnica, foi necessário compreender o funcionamento operacional hospitalar, incluindo:

* Status dos leitos (ocupado, disponível, bloqueado, manutenção)
* Categorias de leitos (UTI, enfermaria, isolamento, etc.)
* Áreas e setores responsáveis
* Fluxo de movimentação de pacientes
* Responsáveis por limpeza e manutenção
* Origem e estrutura dos relatórios existentes

Esse entendimento foi fundamental para modelar corretamente os dados e gerar análises confiáveis.

---

## 🏗️ Arquitetura do Projeto

O projeto foi dividido em três camadas principais:

```
Base de Dados (Excel / CSV)
        ↓
Tratamento e Análise (Python)
        ↓
Visualização e Dashboard (Power BI)
```

### 1️⃣ Base de Dados

Responsável por armazenar e estruturar os dados brutos.

Arquivos simulados:

* Leitos.csv
* Pacientes.csv

Contém informações como:

* ID do leito
* Status
* Categoria
* ID do paciente
* Datas de entrada e saída
* Eventos de manutenção e limpeza

---

### 2️⃣ Tratamento e Análise de Dados (Python)

Responsável por:

* Limpeza dos dados
* Tratamento de inconsistências
* Criação de novas colunas e métricas
* Geração de indicadores estratégicos
* Criação da tabela de eventos de movimentação

Exemplos de análises realizadas:

* Tempo médio de permanência
* Taxa de ocupação
* Tempo médio de leitos bloqueados
* Frequência de utilização por setor
* Identificação de gargalos

---

### 3️⃣ Visualização de Dados (Power BI)

Responsável por transformar dados em dashboards interativos.

Exemplos de visualizações criadas:

* Taxa de ocupação em tempo real
* Quantidade de leitos disponíveis
* Tempo médio de permanência
* Histórico de movimentações
* Leitos bloqueados por manutenção
* Indicadores de eficiência hospitalar

---

## 🔗 Modelagem e Relação entre Dados

Foram criadas e relacionadas as seguintes tabelas:

### Tabela: Leitos

| Campo     | Descrição                       |
| --------- | ------------------------------- |
| id_leito  | Identificador único             |
| categoria | Tipo do leito                   |
| Local     | Localização                     |
| status    | Disponível, ocupado, manutenção |
| Paciente Associado | Identificador do paciente |
| DataInicio | Data de Entrada |
| DataFim | Data de Saída |

---

### Tabela: Pacientes

| Campo        | Descrição           |
| ------------ | ------------------- |
| id_paciente  | Identificador único |
| idade        | Idade do paciente   |
| Sexo         | Gênero Sexual       |
| faixa        | Infantil e Adulto   |
| Tpo_internacao | UTI, Cirúrgica ou Clínica |

---

### Tabela: Eventos_Movimentacao

Tabela central criada para registrar todos os eventos:

| Campo       | Descrição                            |
| ----------- | ------------------------------------ |
| id_leito    | Leito relacionado                    |
| id_paciente | Paciente relacionado                 |
| data_admissao | Data de Admissão                   |
| data_alta | Data da alta do paciente               |

Essa tabela permite rastrear todo o histórico de utilização dos leitos.

---

## 📊 Indicadores Criados (KPIs)

Principais indicadores desenvolvidos:

* Taxa de ocupação (%)
* Tempo médio de permanência
* Quantidade de leitos disponíveis
* Quantidade de leitos bloqueados
* Taxa de utilização
* Tempo médio de bloqueio
* Eficiência operacional

---

## 🛠️ Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Excel / CSV
* Power BI
* Git e GitHub

---

## 📈 Resultados Esperados

Com este projeto, é possível:

* Melhorar o controle dos leitos
* Reduzir tempo ocioso
* Melhorar comunicação entre equipes
* Identificar gargalos operacionais
* Reduzir perdas financeiras
* Auxiliar gestores na tomada de decisão

---

## 🚀 Possíveis Melhorias Futuras

* Integração com banco de dados real (PostgreSQL ou SQL Server)
* Atualização em tempo real
* Criação de API para acesso aos dados
* Sistema web para controle hospitalar
* Previsão de ocupação usando Machine Learning

---

## 💡 Conclusão

Este projeto demonstra como a análise de dados pode ser utilizada para resolver problemas reais, melhorar processos operacionais e gerar valor estratégico.

Além disso, evidencia habilidades em:

* Análise de dados
* Tratamento de dados
* Modelagem de dados
* Criação de indicadores
* Visualização de dados
* Pensamento analítico aplicado a problemas reais

---

