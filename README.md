# Análise Exploratória de Dados — Empresas Cadastradas no Programa

Análise exploratória de uma base com 3.211 empresas cadastradas, com foco no agronegócio, no ecossistema de inovação e no município de Ribeirão Preto (SP).

---

## Arquivos do repositório

| Arquivo | Descrição |
|---|---|
| `auspin_refatorado.ipynb` | Notebook principal com toda a análise |
| `mapa_sp_faturamento.html` | Mapa interativo de faturamento por município — abra no navegador |
| `README.md` | Este arquivo |

---

## Sobre os dados

A base contém informações cadastrais e financeiras de empresas, com as seguintes colunas:

| Coluna | Descrição |
|---|---|
| Nome fantasia | Nome comercial da empresa |
| Ano de fundação | Ano em que a empresa foi fundada |
| CNAE | Classificação Nacional de Atividades Econômicas |
| Cidade | Município de atuação |
| Estado | Unidade federativa ou país |
| Descrição | Breve descrição da empresa e seu ramo |
| Faturamento | Faturamento declarado no último ano |

### Privacidade

Os dados utilizados referem-se exclusivamente a pessoas jurídicas. A LGPD (Lei nº 13.709/2018) protege dados de pessoas naturais, portanto esses registros estão fora do escopo de proteção da lei. Colunas com informações de contato foram removidas antes do início da análise.

---

## Dados

A base de dados não está disponível neste repositório por restrições de uso institucional.
Para reproduzir a análise, substitua o arquivo `empresas_dna.xlsx` por uma base
com as mesmas colunas descritas acima.

---

## O que foi analisado

**Visão geral da base**
- Distribuição de faturamento com identificação de outliers
- Evolução histórica de abertura de empresas por ano
- Distribuição geográfica por estado com escala logarítmica
- Mapa interativo de faturamento médio por município em SP

**Agronegócio**
- Identificação de 227 empresas do setor por CNAE e filtragem por descrição
- Nuvem de palavras com o vocabulário predominante nas descrições

**Ribeirão Preto**
- Distribuição por setor das 267 empresas da cidade
- Faturamento médio por setor
- Detalhamento das 22 empresas do agronegócio presentes na cidade

**Pesquisa e Desenvolvimento (CNAE 72)**
- Crescimento de empresas de P&D por ano de fundação
- Concentração geográfica — Ribeirão Preto é o segundo maior polo do estado
- Vocabulário de inovação nas descrições das empresas

**Comparativo Agtech vs. Agro Tradicional**
- Quantidade de empresas e faturamento médio por grupo

---

## Como executar

### Requisitos

```bash
pip install pandas matplotlib seaborn geopandas folium wordcloud openpyxl jupyter
```

### Executando o notebook

```bash
jupyter notebook auspin_refatorado.ipynb
```

### Mapa interativo

Abra o arquivo `mapa_sp_faturamento.html` diretamente no navegador. Não é necessário instalar nada.

---

## Tecnologias utilizadas

- Python 3.10+
- pandas, numpy
- matplotlib, seaborn
- geopandas, folium
- wordcloud
