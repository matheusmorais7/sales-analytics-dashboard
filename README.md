# 📊 Dashboard Comercial Power BI

assets/dashboard-geral.png

## 🎯 Objetivo

Desenvolver um dashboard comercial completo para análise de desempenho de vendas, acompanhamento de KPIs e monitoramento do funil comercial.

---

## 🚀 Principais Indicadores

✅ Receita Total

✅ Quantidade de Pedidos

✅ Ticket Médio

✅ GM%

✅ Top Vendedor

✅ Produtos Mais Vendidos

✅ Análise por Região

✅ Funil de Conversão Comercial

---

## 🛠 Ferramentas Utilizadas

- Power BI
- Power Query
- DAX
- Excel

---

## 📈 Visualizações

### Visão Geral

assets/dashboard-geral.png

### Funil Comercial

assets/funil-vendas.png

---

## 📌 Medidas DAX Desenvolvidas

### Receita

```DAX
Receita =
SUM(Vendas[Valor])
```

### Ticket Médio

```DAX
Ticket Medio =
DIVIDE(
    [Receita],
    [Quantidade Pedidos]
)
```

### Top Vendedor

```DAX
Top Vendedor =
VAR Ranking =
TOPN(
    1,
    ALL(Vendedores),
    [Receita],
    DESC
)
RETURN
MAXX(
    Ranking,
    Vendedores[Vendedor]
)
```

---

## 📂 Estrutura do Projeto

```text
assets/
data/
docs/
pbix/
README.md
```

---

## 👨‍💻 Autor

Matheus Morais

Aprendiz Comercial com foco em Análise de Dados e Business Intelligence.

Atualmente desenvolvendo projetos utilizando:

- Power BI
- Excel Avançado
- Power Query
- DAX
- Indicadores Comerciais
