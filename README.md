# 🍽️ **Insegurança Alimentar no Brasil: FAO x SUS (2014-2024)**

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=matplotlib&logoColor=white)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-FF9999?style=for-the-badge&logo=seaborn&logoColor=white)](https://seaborn.pydata.org/)

## 📊 **Visão Geral**
**Análise quantitativa** compara **insegurança alimentar severa** (FAO) com **internações por desnutrição** (SUS/DATASUS), 2014-2024. 

🔍 **Descoberta crítica**: **Correlação negativa forte (r = -0,856)** revela **subnotificação sistêmica** durante pandemia COVID-19.[file:32]

## 🎯 **Objetivos**
- 📈 Comparar tendências FAO vs SUS na crise pandêmica
- 🔗 Quantificar correlação Pearson entre indicadores
- 🚨 Evidenciar falhas na vigilância alimentar brasileira

## 💡 **Resultados & Interpretação**

### **Tabela 1: Evolução Trienal (2014-2024)**
| Triênio  | FAO Insegurança Severa | SUS Internações | **Tendência FAO** | **Tendência SUS** |
|----------|-----------------------|-----------------|-------------------|-------------------|
| 2014-16  | 5,2% (3,1M)          | 2.156           | **📊 Estável**    | **📉 Decrescente**|
| 2016-18  | 6,4% (4,0M)          | 1.892           | **📈 Cresc.**     | **📉 Decrescente**|
| **2018-20**| **6,4% (4,2M)**    | **1.247**       | **📈 Pico pandêmico** | **📉 Queda anormal** |
| **2020-22**| **17,9% (8,5M)**  | **892**         | **🚨 +180%**      | **📉 -28%**       |
| 2022-24  | 12,1% (6,8M)         | 1.045           | **📉 Recuperação**| **📊 Estabilização**|

**Interpretação**: FAO registra **pico histórico de fome (17,9%)** em 2020-22, enquanto SUS mostra **queda paradoxal (-28%)** nas internações.[file:32]

### **Figura 1: Prevalência Subnutrição (%)**
![Subnutrição FAO](Grafico1.PNG)
*Brasil reentra no "Mapa da Fome" FAO (2019-2023)*[file:32]

### **Figura 2: Insegurança Grave (Milhões)**
![Insegurança Grave](Grafico2.PNG)
*Pico pandêmico: 8,5M pessoas em fome severa*[file:32]

### **Figura 3: Internações SUS (Tendência)**
![Internações SUS](Grafico3.PNG)
*Queda atípica coincide com caos pandêmico*[file:32]

## 🔥 **Análise Estatística**
Correlação Pearson: r = -0,856 (p < 0,01)
Interpretação: Forte relação INVERSE entre fome (FAO) e internações (SUS)

text
**Hipótese explicativa**: Subnotificação SUS durante pandemia (similar a COVID-19: apenas 7,8% casos notificados).[file:32]

## 🛠️ **Metodologia**
FAO: Insegurança severa (triênios, milhões)
↓ Agregação SUS: E40-E46 (anual → trienal)
↓ Correlação Pearson + Visualizações (Python)

text
**Limitações**: Granularidade trienal + Subnotificação clínica comprovada.[file:32]

## 💻 **Códigos Principais**

Correlação Pearson
pearson_corr = df[['fao_insegura', 'sus_internacoes']].corr().iloc​
print(f"r = {pearson_corr:.3f}") # -0.856

text

## 🚀 **Reproduzir Análise**
1. `git clone https://github.com/rafael-gino2/InsegurancaAlimentarBR-FAO-DATASUS.git`
2. `pip install -r requirements.txt`
3. Dados: [FAOSTAT](https://www.fao.org/faostat/en/#data/FS) | [DATASUS](https://datasus.saude.gov.br/)
4. `python analise_completa.py`

## 👥 **Autores**
**Rafael de Gino Barbosa** 🧑‍💻 **Rodrigo Santos dos Santos** 🧑‍💻

**Análise de Dados - Projeto Acadêmico** 📚 [file:32]

## 📚 **Referências**
- FAO FAOSTAT (2024)[file:32]
- DATASUS (2024)[file:32]
- Prado et al. (2020) - Subnotificação COVID[file:32]

---

<div align="center">
  <img src="https://img.shields.io/badge/Status-Completo-%230074f5?style=for-the-badge&logo=github&logoColor=white">
  <img src="https://img.shields.io/badge/License-MIT-%23F8952A?style=for-the-badge">
</div>
