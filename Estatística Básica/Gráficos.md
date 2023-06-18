# Gráficos

A representação gráfica de distribuição de uma variável tem a vantagem de rápida e concisamente, informar sobre sua variabilidade.

## Gráficos para variáveis qualitativas

Existem vários tipos de gráficos para representar variáveis qualitativas, vários são versões diferentes do mesmo princípio sendo os principais o gráfico de barras e o gráfico de pizza.

```python
import matplotlib.pyplot as plt
plt.bar(df["Grau de Instrução"].value_counts().index, df["Grau de Instrução"].value_counts().values)
plt.title("Gráfico em barras para a variável y: grau de instrução")
plt.ylabel("Frequência")
plt.show()
```

![[Gráfico de barras.png]]

```python
plt.pie(df["Grau de Instrução"].value_counts().values, labels=df["Grau de Instrução"].value_counts().index, autopct='%1.1f%%')
plt.title("Gráfico em barras para a variável y: grau de instrução")
plt.show()
```

![[Pasted image 20230618104825.png]]

