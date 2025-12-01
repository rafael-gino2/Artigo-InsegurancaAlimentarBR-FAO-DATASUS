# 🍽️ Insegurança Alimentar no Brasil: FAO x SUS (2014–2024)

Projeto de análise de dados que investiga a relação entre a insegurança alimentar severa no Brasil, medida pela FAO, e as internações por morbidades nutricionais registradas no SUS (DATASUS), no período de 2014 a 2024.[file:33]

## 📊 Visão geral do estudo

O trabalho cruza séries temporais da FAO (insegurança alimentar severa, em milhões de pessoas por triênio) com dados do DATASUS sobre internações por desnutrição (CID-10 E40–E46), agregados em médias trienais para tornar os indicadores comparáveis.[file:33] O foco é entender o que aconteceu durante os anos da pandemia de COVID-19, quando o Brasil voltou ao “Mapa da Fome” ao mesmo tempo em que os registros clínicos de desnutrição caíram.[file:33]

## 🎯 Pergunta central

A pergunta que orienta o projeto é:  
“Como a evolução da insegurança alimentar severa no Brasil, reportada pela FAO, se relaciona com as internações por desnutrição registradas no SUS entre 2014 e 2024, especialmente durante a pandemia de COVID-19?”[file:33]

## 🛠️ Metodologia de análise

- Extração de dados:
  - FAO/FAOSTAT: população em condição de insegurança alimentar severa, em milhões de pessoas, por triênios.[file:33]
  - DATASUS: internações hospitalares por desnutrição (CID-10 E40 a E46), de 2014 a 2024.[file:33]
- Tratamento:
  - Agregação dos dados anuais do SUS em médias trienais para alinhar à periodicidade da FAO.[file:33]
  - Análise descritiva e exploratória com Python (Pandas, NumPy, Matplotlib, Seaborn).[file:33]
- Estatística:
  - Cálculo da correlação de Pearson entre a série de insegurança alimentar severa (FAO) e a série de internações por desnutrição (SUS).[file:33]

## 📈 Principais resultados

- Os dados da FAO mostram um aumento expressivo da insegurança alimentar severa nos triênios que incluem os anos da pandemia, com a proporção da população em fome severa saltando de 6,4% (2018–2020) para 17,9% (2020–2022).[file:33]
- Paralelamente, as internações por desnutrição no SUS apresentam tendência continuamente decrescente ao longo de todo o período, inclusive nos anos em que a fome mais aumenta.[file:33]
- A correlação de Pearson entre os dois indicadores é forte e negativa (r = -0,856), indicando que, enquanto a insegurança alimentar cresce, os registros clínicos de desnutrição caminham na direção oposta.[file:33]

## 🔍 Interpretação dos gráficos

- ![Subnutrição FAO](Grafico1.PNG)
- (prevalência de subnutrição, FAO): evidencia o retorno do Brasil ao Mapa da Fome a partir do triênio 2019–2021, com patamares de subnutrição mais altos nos triênios pandêmicos.[file:33][image:1]
- ![Insegurança Grave](Grafico2.PNG)
- (pessoas em insegurança alimentar grave): mostra o pico de pessoas em situação de fome severa, atingindo valores históricos durante 2020–2022.[file:33][image:3]
- ![Internações SUS](Grafico3.PNG)
- (internações por desnutrição – SUS): revela uma trajetória de queda nas médias trienais de internações, mesmo quando a insegurança alimentar está em alta.[file:33][image:2]

Essa combinação de curvas (FAO em alta x SUS em queda) reforça a hipótese de subnotificação importante de casos clínicos de desnutrição durante a pandemia.[file:33]

## ⚠️ Limitações discutidas no artigo

- Dados da FAO em triênios, o que reduz a granularidade temporal e pode esconder variações anuais ou sazonais.[file:33]
- Subnotificação clínica e epidemiológica já documentada para a COVID-19 e outras doenças (como dengue e tuberculose), o que sugere cenário semelhante para a desnutrição.[file:33]
- Uso de interpolações em alguns pontos das séries, introduzindo margens de estimativa nas análises.[file:33]

## 🚀 Como reproduzir a análise

1. Clonar o repositório:
git clone https://github.com/rafael-gino2/InsegurancaAlimentarBR-FAO-DATASUS.git

text
2. Instalar dependências:
pip install -r requirements.txt

text
3. Baixar ou conferir os dados originais:
- FAOSTAT (FAO) – indicadores de segurança alimentar.[file:33]
- DATASUS – internações hospitalares por CID-10.[file:33]
4. Executar o script principal:
python analise_completa.py

text

## 👥 Autores

Rafael de Gino Barbosa  
Rodrigo Santos dos Santos[file:33]

Projeto acadêmico de Análise de Dados sobre insegurança alimentar, morbidades nutricionais e qualidade dos sistemas de informação em saúde no Brasil.[file:33]
