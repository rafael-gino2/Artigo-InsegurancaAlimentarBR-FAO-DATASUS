# 🍽️ **Insegurança Alimentar no Brasil: FAO x SUS (2014-2024)**

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=matplotlib&logoColor=white)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-FF9999?style=for-the-badge&logo=seaborn&logoColor=white)](https://seaborn.pydata.org/)

## 📊 **Visão Geral**
**Análise quantitativa** da relação entre **insegurança alimentar severa** (FAO) e **internações por desnutrição** (SUS/DATASUS) no Brasil, 2014-2024. 

🔍 **Descoberta principal**: Correlação negativa forte (**r = -0,856**) sugere **subnotificação massiva** durante a pandemia COVID-19.

![Pandemia Impacto](insira-aqui-figura-pandemia.png)

## 🎯 **Objetivos**
- 📈 Comparar tendências FAO vs SUS durante crise pandêmica
- 🔗 Calcular correlação entre indicadores nutricionais  
- 🚨 Evidenciar falhas na vigilância alimentar brasileira

## 🛠️ **Metodologia**
FAO: Insegurança alimentar severa (triênios, milhões pessoas)
↓
SUS: Internações CID-10 E40-E46 (anual → trienal agregado)
↓
Python + Pandas/NumPy/Seaborn → Correlação Pearson

text

**⚠️ Limitações**: Subnotificação clínica + falta granularidade temporal

## 💻 **Códigos Python Utilizados**

### 1. **Carregamento e Preparação**
Cole seu código de importação e limpeza aqui
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

Seu código de carregamento FAO e SUS aqui...
text

### 2. **Agregação Trienal SUS**
Cole seu código de agregação aqui
Exemplo: sus_data.groupby(['ano_inicio', 'ano_fim']).agg({'internacoes': 'mean'})
text

### 3. **Correlação e Visualizações**
Cole seu código de correlação Pearson aqui
pearson_corr = df[['fao_insegura', 'sus_internacoes']].corr().iloc
text

## 📈 **Gráficos Gerados**

### **Figura 1: Subnutrição por Triênios (FAO)**
![Subnutrição FAO](<img width="333" height="218" alt="image" src="https://github.com/user-attachments/assets/b916fbc9-c919-4404-b396-942451c5809a" />)

### **Figura 2: Insegurança Grave (Pandemia)**
![Insegurança Grave](insira-figura2.png)

### **Figura 3: Internações SUS (Tendência Decrescente)**
![Internações SUS](insira-figura3.png)

## 🔥 **Resultados Principais**
| Período   | FAO Insegurança Severa | SUS Internações | Tendência     |
|-----------|----------------------|-----------------|---------------|
| 2018-20   | 6,4% **📈**          | 1.247 **📉**    | **OPOSTAS**   |
| 2020-22   | **17,9%** 📈         | **892** 📉      | **SUBNOTIFICAÇÃO** |

**💡 Insight**: Enquanto FAO registra **picos de fome**, SUS mostra **queda** → **Alerta sistêmico!**

## 🚀 **Como Reproduzir**
1. Clone o projeto
git clone https://github.com/rafael-gino2/InsegurancaAlimentarBR-FAO-DATASUS.git

2. Ambiente
pip install -r requirements.txt

3. Dados originais
📥 FAOSTAT: https://www.fao.org/faostat/en/#data/FS
📥 DATASUS: https://datasus.saude.gov.br/

4. Execute
python analise_completa.py

text

## 👥 **Autores**
**Rafael de Gino Barbosa** 🧑‍💻 **Rodrigo Santos dos Santos** 🧑‍💻

**Projeto acadêmico - Análise de Dados** 📚

## 📚 **Referências**
- [FAO FAOSTAT](https://www.fao.org/faostat/en/#data/FS)
- [DATASUS](https://datasus.saude.gov.br/)
- [State of Food Security 2022](https://www.fao.org/publications/sofi)

---

<div align="center">
  <img src="https://img.shields.io/badge/Status-Completo-%230074f5?style=for-the-badge&logo=github&logoColor=white" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-%23F8952A?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSI5NCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDkwIDI0Ij48L3N2Zz4=">
</div>
