
# 📊 Segmentação de Clientes com K-Means

Este projeto tem como objetivo realizar a **segmentação de clientes com base em características demográficas e padrões de consumo**, utilizando o algoritmo de clusterização K-Means. A proposta é mostrar como técnicas de machine learning não supervisionado podem ser aplicadas para gerar **insights de negócio** e auxiliar estratégias de marketing.

---

## 🎯 Objetivo

Dividir os clientes em **grupos com comportamentos semelhantes**, a fim de personalizar ações de vendas, retenção e campanhas de marketing.

---

## 🧩 Sobre os Dados

- **Fonte:** Base fictícia de clientes de um shopping
- **Colunas principais:**
  - CustomerID
  - Gender
  - Age
  - Annual Income (k$)
  - Spending Score (1-100)

---

## 🧠 Metodologia

1. **Exploração dos Dados (EDA)**
   - Análise estatística e visual das variáveis
2. **Pré-processamento**
   - Normalização dos dados utilizando StandardScaler
3. **Aplicação do Algoritmo K-Means**
   - Definição da quantidade de clusters utilizando o método do cotovelo (Elbow Method)
4. **Visualização dos clusters**
   - Criação de gráficos para análise visual dos grupos
5. **Rotulagem dos Grupos**
   - Interpretação dos perfis de cada cluster com base nos dados

---

## 📈 Resultados

- **4 grupos distintos foram identificados:**
  - Jovens com alto gasto
  - Adultos com renda alta e gasto moderado
  - Clientes com baixa renda e alto score de gastos
  - Clientes mais velhos com baixo engajamento

---

## 🚀 Como Executar o Projeto

1. Clone este repositório:
```bash
git clone https://github.com/Gustavocorreard/segmentacao-clientes-kmeans.git
cd segmentacao-clientes-kmeans
```

2. Crie um ambiente virtual (opcional, mas recomendado):
```bash
python -m venv .venv
source .venv/bin/activate  # Linux ou Mac
.venv\Scripts\activate  # Windows
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

4. Execute o notebook:
- Acesse a pasta `notebooks/`
- Abra o arquivo `segmentacao_kmeans.ipynb` no Jupyter Notebook ou Google Colab
=======
### Radar Chart com Comparação dos Clusters:
![Radar Chart](https://github.com/Gustavocorreard/mall-customers-clustering/blob/main/images/cluster_pca_plot.png)


---

## 📚 Tecnologias e Ferramentas

- Python
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📌 Conclusão

A segmentação de clientes com K-Means é uma ferramenta poderosa para **entender perfis de consumo e comportamento de usuários**. Este projeto simula uma aplicação real de agrupamento de clientes que pode ser usada em diversos contextos comerciais, contribuindo para estratégias de marketing, vendas e relacionamento.

---

## 👨‍💻 Autor

**Gustavo Correard**  
🔗 [LinkedIn](https://www.linkedin.com/in/gustavocorreard/)  
🔗 [GitHub](https://github.com/Gustavocorreard)
=======
- Mesmo com um **Silhouette Score moderado (0.33)**, os clusters identificados apresentaram **coerência de negócio** e permitiram **ações práticas de segmentação**.
- A clusterização identificou grupos altamente engajados e outros com potencial de crescimento, demonstrando o poder da análise não supervisionada em decisões estratégicas.
