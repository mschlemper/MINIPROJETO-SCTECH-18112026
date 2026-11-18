# MiniProjeto DataView: Exploração e Análise de Dados de Vendas

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mschlemper/MINIPROJETO-SCTECH-18112026/blob/main/dataview.ipynb)

## Sobre o projeto
O **DataView** é um projeto de análise exploratória de dados (EDA) de vendas e Engenharia de Dados, desenvolvido em Python utilizando o Google Colab. O fluxo desenvolvido lê, limpa, transforma, analisa e visualiza um dataset de vendas sintético, gerando relatórios úteis, métricas consolidadas, análises de BI e arquivos finais prontos para tomada de decisões gerenciais.

## O que o projeto analisa
* Receita total e volume de vendas por mês e trimestre.
* Top produtos e categorias por receita gerada.
* Desempenho e ticket médio por região geográfica.
* Segmentação de clientes por nível de gasto (Bronze, Prata, Ouro).
* Comparação entre dados brutos, tratados com outliers (v1) e sem outliers (v2).
* Exportação de relatórios analíticos estruturados em CSV e JSON.

## Diferenciais do Pipeline Técnico
* **Limpeza Avançada:** Remoção automática de sujeiras em strings com expressões regulares (Regex) e integridade de datas.
* **Tratamento de Outliers (IQR):** Algoritmo matemático para detecção de anomalias baseado em amplitude interquartílica, removendo ruídos sem intervenção manual.
* **Estatística Vetorizada:** Processamento e broadcasting com NumPy para computação rápida de percentis e distribuição de receitas.

## Como Executar e Reproduzir
O projeto foi planejado para ser executável de ponta a ponta sem configurações manuais complexas:
1. Acesse o notebook pelo link do Colab no topo desta documentação ou baixe o arquivo `.ipynb` do repositório.
2. Execute todas as células em ordem sequencial.
3. Todos os diretórios (`data/` e `outputs/`) e arquivos serão automaticamente criados, processados e salvos localmente.

## Estrutura de pastas gerada
```text
projeto/
├── data/
│   ├── raw/                  # Dataset original (bruto/sujo)
│   ├── processed/
│   │   ├── v1_com_outliers/  # Dados limpos geral com outliers mantidos
│   │   └── v2_outliers_tratado/ # Dados limpos geral com outliers removidos (IQR)
│   └── final/                # Dataset consolidado final (usado no pipeline final)
├── outputs/
│   ├── metricas_por_mes.csv
│   ├── segmentacao_clientes.csv
│   ├── estatisticas_gerais.json
│   └── graficos/
│       ├── receita_por_mes.png
│       ├── top_produtos.png
│       └── dist_regiao.png
└── README.md
```

## Ferramentas utilizadas
* **Linguagem:** Python 3.10+
* **Bibliotecas:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `re`, `datetime`, `os`, `json`, `random`
* **Controle de Versão:** GitHub
