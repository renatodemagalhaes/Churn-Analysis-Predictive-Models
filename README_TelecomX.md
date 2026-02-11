
# 📊 Telecom X – Previsão de Churn de Clientes - Modelos Preditivos

## 🎯 Propósito da Análise
O objetivo principal deste projeto é **prever o churn de clientes da Telecom X**, ou seja, identificar quais clientes têm maior probabilidade de cancelar seus serviços. A análise utiliza variáveis demográficas, contratuais e de uso dos serviços para apoiar decisões estratégicas de retenção de clientes.

---

## 📁 Estrutura do Projeto

```
TelecomX_Churn/
│
├── TelecomX_Churn_2.ipynb          # Notebook principal com toda a análise
├── dados_tratados.csv              # Base de dados tratada e pronta para modelagem
├── README_TelecomX.md              # Documentação do projeto
└── visualizacoes/                  # (Opcional) Gráficos exportados da EDA
```

---

## 🧹 Preparação dos Dados

### Classificação das Variáveis
- **Categóricas:** tipo de contrato, método de pagamento, serviços adicionais, churn
- **Numéricas:** tempo de contrato (tenure), cobrança mensal, cobrança total

### Tratamento e Transformações
- Codificação de variáveis categóricas via **One-Hot Encoding**
- Normalização das variáveis numéricas usando **StandardScaler**
- Remoção de valores ausentes e inconsistências

### Separação dos Dados
Os dados foram divididos em:
- **Treino:** 70%
- **Teste:** 30%

Utilizando `train_test_split` com `random_state` para reprodutibilidade.

---

## 🤖 Modelagem e Justificativas

Modelos avaliados:
- Regressão Logística
- Random Forest

A **Regressão Logística** foi escolhida como modelo final por:
- Boa interpretabilidade
- Desempenho consistente
- Facilidade de explicação para áreas de negócio

As métricas utilizadas incluem:
- Acurácia
- Precisão
- Recall
- F1-score
- Matriz de confusão

---

## 📈 Análise Exploratória de Dados (EDA)

Durante a EDA, foram identificados insights importantes, como:
- Clientes com contratos mensais apresentam maior churn
- Menor tempo de permanência está fortemente associado ao churn
- Cobranças mensais mais altas tendem a aumentar a evasão

### Exemplos de Gráficos
- Distribuição de churn por tipo de contrato
- Boxplot de cobrança mensal vs churn
- Heatmap de correlação entre variáveis numéricas

---

## ▶️ Como Executar o Projeto

### 1️⃣ Instalar Dependências
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 2️⃣ Executar o Notebook
Abra o arquivo abaixo no Jupyter Notebook ou Jupyter Lab:
```
TelecomX_Churn_Completo.ipynb
```

### 3️⃣ Carregar os Dados
O notebook já está configurado para ler o arquivo:
```python
dados = pd.read_csv("dados_tratados.csv")
```

---

## 📌 Próximos Passos
- Otimização de hiperparâmetros
- Avaliação com outros modelos (XGBoost, LightGBM)
- Deploy do modelo

## 👤 Autor

Renato Magalhães - renatodemagalhaes@yahoo.com.br

Project Link: [https://github.com/renatodemagalhaes/Churn-Analysis-Predictive-Models]

Projeto desenvolvido como parte de um **portfólio profissional em Data Science**, com foco em análise de dados, pensamento analítico e resolução de problemas de negócio.

📫 Aberto a feedbacks, colaborações e oportunidades.

---

⭐ Se este projeto agregou valor ou despertou interesse, fique à vontade para explorar os notebooks!
