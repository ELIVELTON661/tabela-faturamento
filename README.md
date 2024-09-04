import pandas as pd
import pandas as pd

# Dados fornecidos
data = {
    "Ano": [2024, 2024, 2024, 2024, 2024, 2024, 2024, 2023, 2023, 2023],
    "Mês": ["Junho", "Março", "Maio", "Julho", "Janeiro", "Fevereiro", "Abril", "Janeiro", "Setembro", "Outubro"],
    "Faturamento_bruto": [10650, 9550, 11750, 11150, 9500, 11180, 10350, 10500, 9100, 11500],
    "Despesas": [2170, 2250, 2340, 2050, 2160, 2860, 2430, 2550, 2180, 2350],
    "Faturamento_liquido": [8480, 7300, 9410, 9100, 7340, 8320, 7920, 7950, 6920, 9150],
    "Lucro_investimento": [2544, 2190, 2823, 2730, 2202, 2496, 2376, 2385, 2076, 2745],
    "Lucro_salario": [5936, 5110, 6587, 6370, 5138, 5824, 5544, 5565, 4844, 6405]
}

# Criar o DataFrame
df = pd.DataFrame(data)

# Exibir o DataFrame
print(df)
# Criar DataFrame
df = pd.DataFrame(data)

# Uniformizar os meses em letras maiúsculas
df['Mês'] = df['Mês'].str.capitalize()

# Ordenar por Ano e Mês
df['Mês'] = pd.Categorical(df['Mês'], categories=["Janeiro", "Fevereiro", "Março", "Abril", "Maio", "Junho", "Julho", "Agosto", "Setembro", "Outubro", "Novembro", "Dezembro"], ordered=True)
df = df.sort_values(by=['Ano', 'Mês']).reset_index(drop=True)

# Exibir o DataFrame ajustado
print(df)
import pandas as pd

# Dados fornecidos
data = {
    "Ano": [2024, 2024, 2024, 2024, 2024, 2024, 2024, 2023, 2023, 2023],
    "Mês": ["Junho", "Março", "Maio", "Julho", "Janeiro", "Fevereiro", "Abril", "Janeiro", "Setembro", "Outubro"],
    "Faturamento_bruto": [10650, 9550, 11750, 11150, 9500, 11180, 10350, 10500, 9100, 11500],
    "Despesas": [2170, 2250, 2340, 2050, 2160, 2860, 2430, 2550, 2180, 2350],
    "Faturamento_liquido": [8480, 7300, 9410, 9100, 7340, 8320, 7920, 7950, 6920, 9150],
    "Lucro_investimento": [2544, 2190, 2823, 2730, 2202, 2496, 2376, 2385, 2076, 2745],
    "Lucro_salario": [5936, 5110, 6587, 6370, 5138, 5824, 5544, 5565, 4844, 6405]
}

# Criar o DataFrame
df = pd.DataFrame(data)

# Imprimir o DataFrame
print(df)
import pandas as pd

# Dados fornecidos
data = {
    "Ano": [2024, 2024, 2024, 2024, 2024, 2024, 2024, 2023, 2023, 2023],
    "Mês": ["Junho", "Março", "Maio", "Julho", "Janeiro", "Fevereiro", "Abril", "Janeiro", "Setembro", "Outubro"],
    "Faturamento_bruto": [10650, 9550, 11750, 11150, 9500, 11180, 10350, 10500, 9100, 11500],
    "Despesas": [2170, 2250, 2340, 2050, 2160, 2860, 2430, 2550, 2180, 2350],
    "Faturamento_liquido": [8480, 7300, 9410, 9100, 7340, 8320, 7920, 7950, 6920, 9150],
    "Lucro_investimento": [2544, 2190, 2823, 2730, 2202, 2496, 2376, 2385, 2076, 2745],
    "Lucro_salario": [5936, 5110, 6587, 6370, 5138, 5824, 5544, 5565, 4844, 6405]
}

# Criar o DataFrame
df = pd.DataFrame(data)

# Definir a coluna 'Mês' como categórica e ordenar
df['Mês'] = pd.Categorical(df['Mês'], categories=["Janeiro", "Fevereiro", "Março", "Abril", "Maio", "Junho", "Julho", "Agosto", "Setembro", "Outubro", "Novembro", "Dezembro"], ordered=True)

# Ordenar o DataFrame por 'Ano' e 'Mês'
df = df.sort_values(by=['Ano', 'Mês']).reset_index(drop=True)

# Imprimir o DataFrame
print(df)
df['Mês'] = pd.Categorical(
    df['Mês'], 
    categories=[
        "Janeiro", "Fevereiro", "Março", "Abril", "Maio", 
        "Junho", "Julho", "Agosto", "Setembro", "Outubro", 
        "Novembro", "Dezembro"
    ], 
    ordered=True
)
import pandas as pd

# Imprimir o DataFrame antes da alteração
print(df)

# Definir a coluna 'Mês' como categórica e ordenar
df['Mês'] = pd.Categorical(
    df['Mês'], 
    categories=[
        "Janeiro", "Fevereiro", "Março", "Abril", "Maio", 
        "Junho", "Julho", "Agosto", "Setembro", "Outubro", 
        "Novembro", "Dezembro"
    ], 
    ordered=True
df['Mês'] = pd.Categorical( df['Mês'], categories=[ "Janeiro", "Fevereiro", "Março", "Abril", "Maio", "Junho", "Julho", " Agosto", "Setembro", "Outubro", "Novembro", "Dezembro" ], ordered=Verdadeiro )  
