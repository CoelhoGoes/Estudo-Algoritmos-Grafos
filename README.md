# 🚚 Sistema de Logística Urbana - Estudo de Teoria dos Grafos

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Projeto universitário sobre **Teoria dos Grafos** aplicada a um cenário real de logística urbana. Implementação didática de algoritmos clássicos de busca e caminho mínimo em grafos.

## 📋 Descrição do Projeto

Este projeto simula um **Sistema de Logística Urbana** onde uma empresa de entregas precisa otimizar suas rotas partindo de um Depósito Central para diversos pontos da cidade.

### Estrutura do Grafo

- **16 Vértices**: Representam pontos de interesse da cidade (Depósito Central + 15 bairros/locais)
- **Arestas Direcionadas**: Representam as estradas que conectam os pontos
- **Pesos**: Tempo de viagem em minutos entre os pontos
- **Aresta Negativa**: Um "Túnel Expresso" que economiza tempo (demonstra a diferença entre Dijkstra e Bellman-Ford)

### Algoritmos Implementados

#### 🔍 Busca Cega (Não Informada)

- **BFS (Busca em Largura)**: Encontra o caminho com menor número de paradas
- **DFS (Busca em Profundidade)**: Explora o grafo em profundidade

#### ⚡ Caminho Mínimo

- **Dijkstra**: Encontra o caminho de menor tempo (não funciona com pesos negativos)
- **Bellman-Ford**: Encontra o caminho de menor tempo (funciona com pesos negativos e detecta ciclos negativos)

## 🛠️ Tecnologias Utilizadas

- **Python 3.8+**
- **Jupyter Notebook**
- **NetworkX**: Manipulação e análise de grafos
- **Matplotlib**: Visualização de grafos

## 📦 Instalação

### Pré-requisitos

Certifique-se de ter o Python 3.8 ou superior instalado:

```bash
python --version
```

### 1. Clone o repositório

```bash
git clone https://github.com/CoelhoGoes/Estudo-Algoritmos-Grafos.git
cd Estudo-Algoritmos-Grafos
```

### 2. Crie um ambiente virtual (recomendado)

**Windows (PowerShell):**

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

**Linux/macOS:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Instale as dependências

```bash
pip install jupyter networkx matplotlib
```

Ou, se houver um arquivo `requirements.txt`:

```bash
pip install -r requirements.txt
```

## 🚀 Como Executar

### Opção 1: Jupyter Notebook (Recomendado)

1. Inicie o Jupyter Notebook:

```bash
jupyter notebook
```

1. No navegador que abrir automaticamente, clique em `Algoritmos.ipynb`

1. Execute as células sequencialmente:
   - Clique em uma célula e pressione `Shift + Enter` para executá-la
   - Ou use o menu `Cell > Run All` para executar todas as células

### Opção 2: VS Code

1. Abra o projeto no VS Code
2. Instale a extensão "Jupyter" da Microsoft
3. Abra o arquivo `Algoritmos.ipynb`
4. Clique em "Run All" ou execute célula por célula

### Opção 3: Google Colab

1. Acesse [Google Colab](https://colab.research.google.com/)
2. Faça upload do arquivo `Algoritmos.ipynb`
3. Execute as células normalmente

## 📂 Estrutura do Projeto

```text
Estudo-Algoritmos-Grafos/
│
├── Algoritmos.ipynb          # Notebook principal com implementações
├── README.md                 # Este arquivo
└── .gitignore               # Arquivos ignorados pelo Git
```

## 📊 Conteúdo do Notebook

### Célula 1: Introdução

- Descrição do cenário e objetivos do projeto

### Célula 2: Criação do Grafo

- Importação de bibliotecas
- Definição dos 16 vértices
- Criação das arestas com pesos
- Inclusão da aresta negativa (Túnel Expresso)

### Célula 3: Visualização

- Plotagem do grafo com NetworkX
- Destaque visual da aresta negativa

### Células 4-5: Algoritmos de Busca Cega

- Explicação teórica sobre BFS e DFS
- Implementação comentada linha a linha

### Células 6-8: Algoritmos de Caminho Mínimo

- Explicação teórica sobre Dijkstra e Bellman-Ford
- Implementações detalhadas com comentários
- Comparação entre os algoritmos

### Células 9-10: Análise Comparativa

- Execução de todos os algoritmos
- Comparação de resultados
- Demonstração prática das diferenças

## 🎯 Casos de Teste

O notebook executa testes comparativos com:

- **Origem**: Depósito Central (vértice 0)
- **Destino**: Zona Leste (vértice 15)

### Resultados Esperados

- **BFS**: Encontra o caminho com menos arestas
- **DFS**: Mostra a ordem de exploração dos nós
- **Dijkstra**: Encontra o caminho de menor tempo (pode não considerar a aresta negativa corretamente)
- **Bellman-Ford**: Encontra o caminho de menor tempo (considerando a aresta negativa)

## 📚 Conceitos Abordados

### Estruturas de Dados

- Fila (Queue) - BFS
- Pilha (Stack) - DFS
- Fila de Prioridade (Heap) - Dijkstra
- Relaxamento de arestas - Bellman-Ford

### Complexidade de Algoritmos

- **BFS/DFS**: O(V + E)
- **Dijkstra**: O(E log V)
- **Bellman-Ford**: O(V × E)

## ✨ Autores

- **Gabriel Coelho** - [CoelhoGoes](https://github.com/CoelhoGoes)

### Cauê Barroso

- GitHub: [@cauebarroso](https://github.com/cauebarroso)

### Bernardo Lins

- GitHub: [@Bernard0Lins](https://github.com/Bernard0Lins)

## 📝 Licença

Este projeto foi desenvolvido para fins educacionais como parte da disciplina de Teoria de Grafos.

---

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!
