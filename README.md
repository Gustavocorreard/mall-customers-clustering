# 🎯 Segmentação de Clientes com Clusterização (K-Means)

Este projeto tem como objetivo realizar a **segmentação de clientes** de um shopping center com base em informações demográficas e comportamentais, utilizando técnicas de **aprendizado não supervisionado** — mais especificamente, **K-Means Clustering**.

---

## 🧠 Motivação

Empresas que conhecem bem o perfil de seus clientes conseguem criar estratégias de marketing mais eficazes, personalizar ofertas e aumentar o engajamento. Este projeto simula uma aplicação real onde a clusterização ajuda a identificar **padrões de consumo e comportamento** de clientes com base em três variáveis simples: idade, renda e score de gastos.

---

## 🗂️ Fonte dos Dados

- Dataset: [Mall Customers](https://www.kaggle.com/datasets/shwetabh123/mall-customers)
- Tamanho: 200 registros
- Colunas utilizadas:
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1-100)`
  - `Gender` (convertida para binária)

---

## 🧪 Tecnologias e Técnicas Utilizadas

- `Python`
- `Pandas` e `NumPy` (manipulação de dados)
- `Matplotlib` e `Seaborn` (visualização)
- `scikit-learn` (pré-processamento, clusterização, avaliação)
- `StandardScaler` (normalização)
- `KMeans` (algoritmo principal)
- `PCA` (redução de dimensionalidade para visualização)
- `Silhouette Score` (validação dos clusters)

---

## 🔍 Etapas do Projeto

1. **Análise Exploratória dos Dados (EDA)**
   - Verificação de distribuições
   - Detecção de outliers
   - Relação entre variáveis

2. **Pré-processamento**
   - Codificação do gênero
   - Normalização das variáveis com `StandardScaler`

3. **Determinação do número ideal de clusters**
   - Método do cotovelo
   - Validação com Silhouette Score

4. **Aplicação do algoritmo K-Means**
   - Clusterização com K=6 (melhor resultado de Silhouette)

5. **Nomeação dos clusters**
   - Criação de perfis interpretáveis para os grupos formados

6. **Redução de dimensionalidade com PCA**
   - Visualização bidimensional dos clusters

---

## 🧬 Perfis Encontrados

| Segmento              | Idade Média | Renda (k$) | Score de Gasto | Características |
|-----------------------|-------------|------------|----------------|-----------------|
| **Maduros Moderados** | 57.2        | 46.8       | 38.7           | Perfil mais velho, consumo moderado |
| **Ricos Conservadores** | 39.0      | 88.3       | 14.4           | Alta renda, mas baixo engajamento |
| **Jovens Gastadores** | 28.4        | 58.2       | 70.7           | Jovens com gasto elevado |
| **Premium Engajados** | 33.2        | 91.0       | 72.1           | Alta renda e alto engajamento |
| **Aspirantes Jovens** | 25.9        | 41.3       | 57.9           | Baixa renda, mas gasto elevado |
| **Experientes Reservados** | 49.9    | 54.3       | 36.5           | Maduros com comportamento discreto |

---

## 📈 Visualizações

### PCA com 2 Componentes:
![Gráfico PCA](images/clusters_pca.png)

### Radar Chart com Comparação dos Clusters:
![Radar Chart](images/radar_clusters.png)

---

## ✅ Conclusões

- Mesmo com um **Silhouette Score moderado (0.33)**, os clusters identificados apresentaram **coerência de negócio** e permitiram **ações práticas de segmentação**.
- A clusterização identificou grupos altamente engajados e outros com potencial de crescimento, demonstrando o poder da análise não supervisionada em decisões estratégicas.