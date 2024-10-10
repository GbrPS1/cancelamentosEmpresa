# Python Insights - Analisando Dados com Python 📊  
### Case - Cancelamento de Clientes

## 📋 Descrição do Projeto

Este projeto foi desenvolvido para analisar os dados de cancelamento de clientes de uma empresa com mais de **800 mil clientes**. A empresa identificou que uma grande parte da sua base está inativa, ou seja, os clientes cancelaram os serviços. O objetivo do projeto é identificar as causas principais desses cancelamentos e propor soluções eficazes para reduzir o número de clientes que abandonam o serviço.

## 🔍 Objetivo

A análise dos dados se concentra em encontrar os principais motivos que levam os clientes a cancelarem o serviço. Através de visualizações e estatísticas, identificamos três fatores críticos associados ao cancelamento:

1. **Clientes com contratos mensais** têm uma taxa de cancelamento de 100%.
2. **Clientes que ligam mais de 4 vezes para o call center** tendem a cancelar.
3. **Clientes que atrasaram o pagamento por mais de 20 dias** acabam cancelando o serviço.

## 📂 Estrutura do Projeto

```bash
├── cancelamentos_sample.csv  # Dados de cancelamento dos clientes
├── analise_cancelamentos.ipynb  # Notebook principal com análise de dados
└── README.md  # Este arquivo
```

## 📊 Ferramentas Utilizadas

- **Pandas**: Manipulação e exibição de dados.
- **Plotly Express**: Visualização de dados interativa, usada para criar gráficos como histogramas.
- **Jupyter Notebook**: Ambiente para desenvolvimento de scripts e visualização de resultados.

## 🛠️ Metodologia

### 1. Leitura dos Dados

Os dados foram carregados a partir do arquivo `cancelamentos_sample.csv`, que contém informações detalhadas sobre os clientes, como tipo de contrato, número de interações com o call center e dias de atraso no pagamento.

```python
import pandas as pd

# Carregando os dados
tabela = pd.read_csv('cancelamentos_sample.csv')
display(tabela)
```

### 2. Visualização de Dados

Usamos `plotly.express` para criar gráficos interativos que nos ajudaram a entender o comportamento dos cancelamentos em relação aos diferentes fatores.

#### Exemplo: Histograma dos clientes com base no número de ligações para o call center.

```python
import plotly.express as px
```

### 3. Identificação dos Motivos de Cancelamento

- **Clientes com contratos mensais**: Todos os clientes que possuem contratos mensais cancelam o serviço.
- **Número de ligações para o call center**: Clientes que ligaram mais de 4 vezes ao suporte têm alta taxa de cancelamento.
- **Atrasos no pagamento**: Clientes que atrasam mais de 20 dias nas suas faturas cancelam o serviço.

### 4. Soluções Propostas

Com base na análise, foram sugeridas três soluções principais:

1. **Oferecer desconto nos planos anuais e trimestrais**: Incentivar os clientes a migrar de contratos mensais para planos de maior duração, com descontos, para reduzir o risco de cancelamento.
   
2. **Melhorar o atendimento ao cliente**: Implementar um processo mais eficiente, onde os problemas dos clientes sejam resolvidos em no máximo 3 ligações. Isso deve reduzir a frustração e melhorar a retenção.

3. **Política de pagamento e cobrança**: Implementar uma política mais proativa para lidar com atrasos, como resolver questões financeiras em até 10 dias, com uma equipe dedicada para contatar os clientes em risco de cancelamento.

## 📈 Conclusão

Através dessa análise, conseguimos identificar os principais fatores que contribuem para o cancelamento dos clientes. As três soluções propostas são ações práticas que podem ser implementadas para melhorar a retenção de clientes:

1. **Descontos em planos de maior duração**.
2. **Atendimento eficiente com resolução rápida**.
3. **Gestão de atrasos proativa**.

Essas ações têm o potencial de reduzir significativamente o número de cancelamentos e melhorar os resultados da empresa.
