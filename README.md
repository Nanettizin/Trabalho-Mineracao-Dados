# 🌍 Análise de Qualidade do Ar e Poluição da Água
> Uma investigação técnica sobre a correlação física entre poluição atmosférica e hídrica em cidades globais utilizando Mineração de Dados.

**Autores:** Gabriel Vinicios Nanetti & Nathan Scremin

---

## 📖 Sobre o Projeto
Este projeto utiliza algoritmos de Machine Learning não supervisionado para analisar dados ambientais de milhares de cidades ao redor do mundo. O objetivo principal foi investigar se existe um padrão oculto conectando a **Qualidade do Ar** com a **Poluição da Água**.

Ao contrário do senso comum que associa apenas riqueza econômica (PIB) à limpeza ambiental, nossos modelos revelaram que a densidade urbana e a gestão integrada são fatores mais determinantes.

### 📄 Nota Importante
Este repositório contém o código e os dados brutos. Para uma explicação detalhada da metodologia, embasamento teórico (como a Deposição Atmosférica) e interpretação profunda dos resultados, **consulte o artigo/apresentação disponível na pasta `presentation/`**. O PDF entrega as melhores explicações sobre o fenômeno físico descoberto.

---

## 🔍 Principais Descobertas
Através da aplicação de **K-Means** e **Regras de Associação (Apriori)**, identificamos:

1.  **O Cluster da "Crise Dupla":** Megalópoles ricas (como Nova York e Londres) compartilham perfis de alta poluição com cidades em desenvolvimento, provando que o PIB não blinda cidades contra a degradação ambiental.
2.  **A Regra dos 60% (Apriori):** Encontramos uma forte regra de associação (Confiança: 60%) indicando que **"Se a Poluição da Água é Muito Baixa -> A Qualidade do Ar tende a ser Muito Alta"**.
3.  **Validação Científica:** Os dados estatísticos corroboram o fenômeno da **Deposição Úmida**, onde a chuva "lava" poluentes do ar e contamina os recursos hídricos urbanos.

---

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Análise e Manipulação:** Pandas, NumPy
* **Visualização de Dados:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-learn (K-Means, StandardScaler)
* **Mineração de Dados:** Mlxtend (Apriori, Association Rules)

---

## 📂 Estrutura do Repositório

```text
├── data/
│   └── cities_air_quality_water_pollution.csv  # Dataset original utilizado
│
├── notebooks/
│   └── analysis_clustering_apriori.ipynb       # Código completo (Limpeza, K-Means, Apriori)
│
├── presentation/
│   └── presentation_slides.pdf                 # [IMPORTANTE] Artigo com as explicações detalhadas e conclusões
│
└── requirements.txt                            # Lista de dependências para rodar o projeto
