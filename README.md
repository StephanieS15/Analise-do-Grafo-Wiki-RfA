# Análise Estrutural e Algorítmica da Rede de Votação Wiki-RfA

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![NetworkX](https://img.shields.io/badge/NetworkX-Graph_Analysis-orange.svg)](https://networkx.org/)

Repositório contendo os scripts, bases de dados tratadas e o relatório técnico do projeto de análise de redes complexas, focado na base de dados **Wiki-RfA** (Wikipedia Requests for Adminship), extraída do repositório SNAP de Stanford.


## Objetivos Alcançados:
* **Limpeza e Estruturação:** Conversão de um multigrafo temporal bruto em um grafo simples estático (isolamento da maior componente conexa e remoção de self-loops).
* **Extração de Métricas:** Cálculo de dimensão, densidade, distribuição de graus, diâmetro, raio e clusterização.
* **Análise de Desempenho:** Testes comparando o tempo de execução local de algoritmos como **BFS, DFS, Dijkstra, Tarjan e Kruskal** com seus limites teóricos (Big-O).
* **Teste de Robustez:** Simulação de resiliência da rede contra remoção aleatória de nós (5%) versus ataques direcionados aos maiores *hubs* (5%).

## Tecnologias Utilizadas

* **Python 3**
* **NetworkX:** Para modelagem e cálculo de métricas estruturais.
* **Matplotlib / Seaborn:** Para a geração e visualização gráfica dos dados.
* **Pandas:** Para manipulação da base de dados bruta.
* **Jupyter Notebook:** Para estruturação do pipeline de forma interativa.

## Estrutura do Repositório

* `analise_wiki_rfa.ipynb`: Script principal em Jupyter Notebook com todo o pipeline (tratamento de dados, métricas, algoritmos e gráficos).
* `wiki-RfA.txt`: Base de dados original bruta contendo o histórico de votações.
* `wiki-RfA_edges_clean.csv`: Base de dados tratada em formato tabular, contendo as arestas limpas após a remoção de loops e redundâncias.
* `wiki-RfA_lista_adjacencia.adjlist`: Arquivo com a estrutura topológica do grafo exportada em formato de lista de adjacência.
* `imagens geradas/`: Pasta com os gráficos exportados durante as análises.
  * `dsitribuicao_graus.png`: Gráfico da distribuição de graus em escala log-log.
  * `representacao_grafo.png`: Visualização estrutural da rede.
* `README.md`: Documentação principal do projeto.

## Como Executar

1. Clone este repositório para sua máquina local:
   ```bash
   git clone [https://github.com/stephaniesacramento/wiki-rfa-graphs.git](https://github.com/stephaniesacramento/wiki-rfa-graphs.git)

2. Configurar o ambiente e dependências

Crie e ative um ambiente virtual (opcional, mas recomendado):

**No Windows:**
```bash
python -m venv venv
venv\Scripts\activate

**No Linux/Mac:**
python3 -m venv venv
source venv/bin/activate

Instale as bibliotecas necessárias para rodar o script:

pip install networkx matplotlib pandas jupyter scipy

4. Rodar a análise

Com tudo instalado, inicie o servidor do Jupyter Notebook:
Bash

jupyter notebook

    O seu navegador abrirá automaticamente.

    Clique no arquivo analise_wiki_rfa.ipynb.

    Vá no menu superior, clique em Cell (ou Run) e selecione Run All para executar todo o pipeline, desde a limpeza dos dados até a geração dos gráficos de resultados.

Autora: Stephanie Sacramento - Universidade Federal da Bahia (UFBA)