# 🏠 Análise Exploratória do Mercado Imobiliário Brasileiro

Análise exploratória de dados (EDA) sobre o mercado de aluguel no Brasil, com foco em Rio de Janeiro e São Paulo. O projeto investiga os principais fatores que influenciam o preço do aluguel residencial.

---

## 📊 Principais Descobertas

| Insight | Detalhe |
|---|---|
| 🏙️ RJ domina o dataset | 5.249 imóveis (86%) vs 831 em SP |
| 💰 RJ tem aluguéis mais altos | Média R$ 4.695 vs R$ 2.506 em SP |
| 🛁 Banheiros explicam mais o preço que a área | Correlação de 0.66 com aluguel |
| 🚗 Mais vagas = mais caro | Correlação de 0.58 com aluguel |
| 🐾 Imóveis pet friendly são ~22% mais caros | R$ 4.586 vs R$ 3.769 de média |
| 📐 Área influencia, mas não é o maior fator | Correlação de apenas 0.24 |

---

## 📁 Estrutura do Projeto

```
imoveis-brasil-eda/
├── data/
│   ├── raw/                  ← dataset original (não modificado)
│   └── processed/            ← dados limpos prontos para análise
├── notebooks/
│   └── analise.ipynb         ← análise completa passo a passo
├── outputs/
│   └── graficos/             ← visualizações geradas
├── requirements.txt
└── README.md
```

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.11**
- **pandas** — manipulação e limpeza dos dados
- **numpy** — operações numéricas
- **matplotlib** — visualizações base
- **seaborn** — gráficos estatísticos

---

## 🚀 Como Rodar Localmente

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/imoveis-brasil-eda.git
cd imoveis-brasil-eda

# Crie o ambiente virtual
python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/Mac

# Instale as dependências
pip install -r requirements.txt

# Abra o notebook
jupyter notebook notebooks/analise.ipynb
```

---

## 📈 Etapas da Análise

1. **Carregamento dos dados** — leitura do dataset com pandas
2. **Limpeza** — remoção de colunas desnecessárias, conversão de tipos, tratamento de nulos e valores com `R$`
3. **Análise exploratória** — distribuições, médias por cidade, correlações
4. **Visualizações** — gráficos de barras, scatter plot, boxplot e heatmap de correlação

---

## 📦 Dataset

- **Fonte:** [Kaggle — Brazilian Houses to Rent](https://www.kaggle.com/datasets/rubenssjr/brasilian-houses-to-rent)
- **Registros:** 6.080 imóveis
- **Cidades:** Rio de Janeiro e São Paulo
- **Variáveis:** área, quartos, banheiros, vagas, andar, condomínio, aluguel, IPTU, seguro, total

---

## 📌 Observações

- O dataset é desbalanceado: Rio de Janeiro representa 86% dos registros, o que pode influenciar comparações entre cidades.
- Outliers foram mantidos na análise geral e removidos apenas nos gráficos de dispersão para melhor visualização.

---

Desenvolvido como parte de um portfólio de Ciência de Dados.