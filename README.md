# Análise de Churn de Clientes - Telecom

## 📌 Descrição do Projeto
Este projeto realiza uma **análise exploratória de dados (EDA)** sobre o comportamento dos clientes de uma empresa de telecomunicações, com foco em entender os padrões de **evasão de clientes (Churn)**.  

O objetivo é identificar características e comportamentos que estejam relacionados ao cancelamento de serviços, auxiliando em estratégias de retenção.

---

## 🗂️ Estrutura do Projeto

- `data/` - Contém os dados brutos (JSON/CSV) dos clientes.  
- `notebooks/` - Notebooks do Google Colab com todo o tratamento, análise e visualizações.  
- `figures/` - Gráficos gerados durante a análise.  
- `README.md` - Este arquivo, com descrição do projeto.

---

## 🧹 Limpeza e Tratamento de Dados
- Conversão do JSON para DataFrame do Pandas.
- Separação de colunas aninhadas (customer, phone, internet, account).
- Conversão de valores numéricos (`Charges.Total`, `Charges.Monthly`) para float.
- Criação de nova coluna `Contas_Diarias` com valor médio diário.
- Padronização de valores negativos e tratamento de inconsistências.
- Verificação de valores ausentes e duplicados.

---

## 📊 Análise Exploratória de Dados (EDA)
### Variáveis Categóricas
- Distribuição de Churn por gênero, tipo de contrato, forma de pagamento e serviços contratados.
- Identificação de perfis com maior tendência à evasão.

### Variáveis Numéricas
- Distribuição de gastos (`Charges.Total`, `Charges.Monthly`) e tempo de contrato (`tenure`).
- Visualização de padrões com boxplots e KDE por Churn.
- Estatísticas descritivas: média, mediana, desvio padrão, quartis.

---

## 💡 Principais Insights
- Clientes com **contrato mensal** têm maior probabilidade de cancelar.
- Clientes com **tenure menor** ou **gastos diários baixos** apresentam maior risco de evasão.
- Métodos de pagamento e serviços contratados influenciam na retenção.
- Existem outliers de clientes de alto gasto que também cancelaram, indicando oportunidades de fidelização.

---

## 📈 Recomendações
1. Desenvolver **programas de fidelização** para clientes de contrato mensal.  
2. Monitorar **padrões de consumo** e identificar clientes de baixo gasto antes que cancelem.  
3. Melhorar serviços adicionais (internet, suporte, dispositivos) para aumentar retenção.  
4. Criar **campanhas personalizadas** com base no perfil dos clientes (gênero, dependentes, serviços contratados).

---

## 🛠️ Tecnologias Utilizadas
- Python 3.12
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

## 🚀 Como Executar
1. Clone o repositório:
```bash
git clone https://github.com/seuusuario/churn-analysis.git

notebooks/Churn_Analysis.ipynb


Conclusão

Este projeto fornece uma visão detalhada do comportamento dos clientes e dos fatores que influenciam a evasão. Os insights obtidos podem ser usados para estratégias de retenção e otimização de serviços na empresa.
