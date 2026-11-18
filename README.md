# MiniProjeto DataView: Exploração e Análise de Dados de Vendas

## Sobre o projeto
O **DataView** é um projeto de análise exploratória de dados (EDA) de vendas, desenvolvido em Python utilizando o Google Colab. O fluxo desenvolvido lê, limpa, transforma, analisa e visualiza um dataset de vendas sintético, gerando relatórios úteis, métricas consolidadas e gráficos para subsidiar tomadas de decisões gerenciais.

## O que o projeto analisa
* Receita total e volume de vendas por mês e trimestre.
* Top produtos e categorias por receita gerada.
* Desempenho e ticket médio por região geográfica.
* Segmentação de clientes por nível de gasto (Bronze, Prata, Ouro).
* Comparação entre dados brutos, tratados com outliers (v1) e sem outliers (v2).
* Exportação de relatórios analíticos em CSV e JSON.

## Objetivo
Praticar e aplicar os seguintes conceitos de programação e análise de dados:
* **Lógica de Programação:** Estruturas de controle, condicionais, repetições, manipulação de strings com Regex (`re.sub`) e tratamento de datas com o módulo `datetime`.
* **Funções e Reutilização:** Modularização de pipelines, funções lambda e funções de ordem superior (callbacks).
* **Manipulação de Dados (Pandas):** Leitura de CSV, limpeza, imputação, filtros complexos e agrupamentos (`groupby`).
* **Operações Vetorizadas (NumPy):** Manipulação de arrays, broadcasting, operações vetorizadas de classificação (`np.select`) e cálculos estatísticos (média, mediana, desvio padrão, percentis).
* **Visualização de Dados (Matplotlib & Seaborn):** Criação, personalização e salvamento em arquivo de gráficos de linha, barra e boxplot.

## Como executar

### No Google Colab (Recomendado)
1. Faça o upload do notebook `dataview.ipynb` no ambiente do Colab.
2. Execute todas as células em ordem sequencial (de cima para baixo).
3. O código gerará automaticamente as pastas e os arquivos de dados necessários.

### Localmente com VS Code
1. Instale o Python 3.10+ e o editor VS Code.
2. Instale as dependências executando o comando abaixo no terminal:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Execute o notebook ou script `dataview.ipynb` localmente.

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

## Vídeo de demonstração
*[Inserir link do Google Drive ou YouTube aqui]*
