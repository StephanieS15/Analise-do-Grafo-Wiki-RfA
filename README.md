# Análise Estrutural e Algorítmica da Rede de Votação Wiki-RfA

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![NetworkX](https://img.shields.io/badge/NetworkX-Graph_Analysis-orange.svg)](https://networkx.org/)

Repositório contendo os scripts, bases de dados tratadas e o relatório técnico do projeto de análise de redes complexas, focado na base de dados **Wiki-RfA** (Wikipedia Requests for Adminship), extraída do repositório SNAP de Stanford.

---

## Objetivos do Projeto

- Realizar o tratamento e a modelagem da base de dados Wiki-RfA;
- Extrair métricas estruturais da rede;
- Avaliar o desempenho de algoritmos clássicos em grafos;
- Investigar a robustez da rede sob diferentes estratégias de remoção de vértices.

---

# Tecnologias Utilizadas

- Python 3
- NetworkX
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# Descrição dos Arquivos

| Arquivo | Descrição |
|----------|-----------|
| `analise_wiki_rfa.ipynb` | Notebook contendo todo o pipeline de análise. |
| `wiki-RfA.txt` | Base de dados original disponibilizada pelo SNAP. |
| `wiki-RfA_edges_clean.csv` | Base tratada após remoção de *self-loops* e arestas duplicadas. |
| `wiki-RfA_lista_adjacencia.adjlist` | Grafo exportado em formato de lista de adjacência. |
| `imagens_geradas/` | Gráficos produzidos durante a análise. |
| `README.md` | Documentação do projeto. |

---

# Como Executar

## 1. Clonar o repositório

```bash
git clone https://github.com/StephanieS15/Analise-do-Grafo-Wiki-RfA.git

```

---

## 2. Criar um ambiente virtual (Opcional)

### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv

source venv/bin/activate
```

---

## 3. Instalar as dependências

```bash
pip install networkx pandas matplotlib seaborn scipy jupyter
```

---

## 4. Executar o Notebook

Inicie o servidor do Jupyter:

```bash
jupyter notebook
```

Em seguida:

1. Abra o arquivo `analise_wiki_rfa.ipynb`;
2. Selecione **Run → Run All Cells**;
3. Aguarde a execução completa do pipeline.

Ao final serão gerados:

- métricas da rede;
- tabelas;
- gráficos;
- resultados dos algoritmos;
- análise de robustez.

---

# Base de Dados

A base utilizada é a **Wiki-RfA (Wikipedia Requests for Adminship)**, disponibilizada pelo em:  https://snap.stanford.edu/data/wiki-RfA.html

Ela representa a rede de votações entre usuários da Wikipédia durante os processos de promoção para administradores.

---

# Resultados Obtidos

O projeto contempla:

- tratamento da base de dados;
- construção do grafo;
- caracterização estrutural da rede;
- distribuição de graus;
- análise da propriedade *Small-World*;
- avaliação da robustez da rede;
- comparação experimental de algoritmos clássicos em grafos.

---

# Autora

**Stephanie Sacramento**

Universidade Federal da Bahia (UFBA)

Disciplina de Teoria dos Grafos