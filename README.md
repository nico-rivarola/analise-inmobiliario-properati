# 🏠 Dashboard Imobiliário – Properati

Este projeto faz parte do meu portfólio de Data Science e tem como objetivo realizar uma análise completa do mercado imobiliário com base nos dados da plataforma Properati, aplicando técnicas de análise exploratória, modelagem preditiva e visualização interativa.

## 🎯 Objetivo do Projeto

O principal objetivo é analisar e prever o preço dos imóveis a partir de variáveis como tipo de imóvel, localização, área, número de quartos e banheiros.
Além disso, foi criado um dashboard interativo no Looker Studio, permitindo explorar as informações de forma visual e dinâmica.

### 🧩 Etapas do Projeto

1. Preparação e Limpeza dos Dados
   
  - Importação e padronização do dataset DS_Proyecto_01_Datos_Properati.csv.
  - Seleção das variáveis relevantes:
  tipo_imovel, preco, superficie_total, quartos, banheiros, cidade, provincia, data_publicacao.
  - Tratamento de valores nulos e padronização de formatos (datas, nomes de colunas e unidades).
  - Exportação da base final tratada para dados_properati_tratados.csv, utilizada no dashboard.

2. Análise Exploratória (EDA)
   
  - Avaliação da distribuição de preços, áreas e tipos de imóveis.
  - Análise da relação entre variáveis com gráficos de dispersão, correlação e boxplots.
  - Identificação de regiões com maior valorização e concentração de imóveis.

3. Modelagem Preditiva (Machine Learning)
   
Modelos aplicados:
  - Regressão Linear
  - Árvore de Decisão
  - Random Forest Regressor
  - 
Métricas obtidas:
  - R²: 0.57 (melhor desempenho com Random Forest)
  - MAE: ~67.000 USD
  - RMSE: ~200.000 USD
    
Interpretação das variáveis mais importantes para a precificação dos imóveis.

4. Visualização de Dados – Dashboard Looker Studio
   
- Criação de um Painel Interativo com KPIs e filtros dinâmicos:
      - Preço médio dos imóveis
      - Preço por m²
      - Número total de imóveis e média de quartos
  
 - Gráficos principais:
      - Barras: preço médio por tipo de imóvel e província
      - Série temporal: evolução do preço médio
      - Mapa interativo: imóveis por região
      - Dispersão: relação entre preço e área total
      
🧠 Principais Insights

As províncias mais caras concentram imóveis de alto padrão e maior metragem.
Departamentos e casas representam a maior parte dos anúncios.
Há uma correlação clara entre área total e preço, com influência significativa da localização.

🛠️ Tecnologias Utilizadas
    Python: Pandas, Matplotlib, Seaborn, Scikit-learn
    Jupyter Notebook
    Google Looker Studio
    Git / GitHub
    Joblib para persistência de modelos
📊 Como Reproduzir

1. Clone o repositório:
  
        git clone https://github.com/seuusuario/properati-dashboard.git
        cd properati-dashboard


2. Execute o notebook principal:

    properati.ipynb → limpeza, EDA e modelagem
    graficos-adicionais.ipynb → análise complementar e visualizações

3. Gere a base tratada:

4. df.to_csv("dados_properati_tratados.csv", index=False)

5. Importe o CSV no Looker Studio e crie o dashboard conforme o guia incluso no projeto.


Nicolás Rivarola
📍 Data Analyst
🔗 LinkedIn https://www.linkedin.com/in/nicolas-rivarola/
