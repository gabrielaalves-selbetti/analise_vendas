# Análise de Vendas — Miniprojeto DSA

Projeto desenvolvido durante o curso **Fundamentos de Python** da [Data Science Academy (DSA)](https://www.datascienceacademy.com.br/).

## Objetivo

Simular e analisar dados de vendas de uma loja fictícia de produtos de tecnologia, aplicando conceitos de manipulação de dados, engenharia de atributos e visualização.

## Dataset

Os dados são gerados sinteticamente pela função `gerar_dados_ficticios()` e contêm **1.000 pedidos** de janeiro a julho de 2026.

| Coluna | Descrição |
|---|---|
| `ID_Pedido` | Identificador único do pedido |
| `Data_Pedido` | Data e hora do pedido |
| `Nome_Produto` | Nome do produto vendido |
| `Categoria` | Categoria do produto |
| `Preco_Unitario` | Preço por unidade (com variação para acessórios) |
| `Quantidade` | Quantidade vendida (1–7 unidades) |
| `ID_Cliente` | Identificador do cliente |
| `Cidade` / `Estado` | Localização da venda |
| `Faturamento` | Receita total por pedido (atributo derivado) |
| `Status_Entrega` | `Rápida` (SP/RJ/MG) ou `Normal` (demais estados) |

**Produtos:** Laptop Gamer, Mouse Vertical, Teclado Mecânico, Monitor Ultrawide, Cadeira Gamer, Headset 7.1, Placa de Vídeo, SSD 1TB

**Cidades:** São Paulo, Rio de Janeiro, Belo Horizonte, Porto Alegre, Salvador, Curitiba, Fortaleza

## Análises Realizadas

1. **Top 10 produtos mais vendidos** — ranking por quantidade total vendida (gráfico de barras horizontal)
2. **Faturamento mensal** — evolução da receita ao longo dos meses (gráfico de linha)
3. **Faturamento por estado** — comparativo entre os 7 estados (gráfico de barras)
4. **Faturamento por categoria** — receita agregada por categoria de produto (gráfico de barras com formatação em R$ K)

## Tecnologias

| Biblioteca | Versão | Uso |
|---|---|---|
| `pandas` | 3.0.3 | Manipulação e agregação de dados |
| `numpy` | 2.4.6 | Geração de números aleatórios e operações numéricas |
| `matplotlib` | 3.10.9 | Geração de gráficos |
| `seaborn` | 0.13.2 | Estilo e paletas de cores para visualizações |

## Como Executar

```bash
# 1. Crie e ative o ambiente virtual
python -m venv venv
.\venv\Scripts\Activate.ps1

# 2. Instale as dependências
pip install -r requirements.txt

# 3. Abra o notebook
jupyter notebook app.ipynb
```

## Estrutura

```
analise_vendas/
├── app.ipynb         # Notebook principal com toda a análise
├── requirements.txt  # Dependências do projeto
└── venv/             # Ambiente virtual (não versionado)
```
