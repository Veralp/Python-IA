
# 🤖 **Classificação com IA: Inteligencia Artificial e previsões**  

Este projeto utiliza modelos de Inteligência Artificial para prever resultados com base em um conjunto de dados. A implementação utiliza algoritmos de aprendizado supervisionado, comparando a **Random Forest** e o **K-Nearest Neighbors (KNN)**.

---

## 🚀 **Passos Principais**  

1. **📊 Preparação dos Dados**  
   - Divisão do conjunto de dados em **treino** e **teste**.  
   - Variáveis preditoras: `x_treino` e `x_teste`.  
   - Variáveis de destino: `y_treino` e `y_teste`.  

2. **🛠️ Criação dos Modelos**  
   - **Random Forest**: Um modelo de árvores de decisão para classificação.  
   - **K-Nearest Neighbors (KNN)**: Um modelo baseado em proximidade entre os dados.  

3. **📚 Treinamento dos Modelos**  
   - Os modelos são ajustados com os dados de treino.  

4. **📈 Avaliação de Desempenho**  
   - Predições são feitas com os dados de teste.  
   - **Acurácia** é calculada para medir a eficácia dos modelos.  

---

## 🧪 **Implementação do Código**  

### 🔌 **Importação de Bibliotecas Necessárias**  
```python  
from sklearn.ensemble import RandomForestClassifier  
from sklearn.neighbors import KNeighborsClassifier  
from sklearn.metrics import accuracy_score  
```  

### ⚙️ **Criação e Treinamento dos Modelos**  
```python  
# Criar os modelos  
modelo_arvoredecisao = RandomForestClassifier()  
modelo_knn = KNeighborsClassifier()  

# Treinar os modelos  
modelo_arvoredecisao.fit(x_treino, y_treino)  
modelo_knn.fit(x_treino, y_treino)  
```  

### 📊 **Predição e Avaliação**  
```python  
# Fazer previsões  
previsao_arvoredecisao = modelo_arvoredecisao.predict(x_teste)  
previsao_knn = modelo_knn.predict(x_teste)  

# Calcular a acurácia  
print("Acurácia - Random Forest:", accuracy_score(y_teste, previsao_arvoredecisao))  
print("Acurácia - KNN:", accuracy_score(y_teste, previsao_knn))  
```  

---

## 📈 **Resultados Esperados**  
O script retorna a acurácia de cada modelo, permitindo escolher o mais eficaz para a tarefa de classificação.  

---

## 📚 **Recursos Utilizados**  
- **RandomForestClassifier**: Modelo de árvores de decisão da biblioteca `sklearn.ensemble`.  
- **KNeighborsClassifier**: Algoritmo KNN da biblioteca `sklearn.neighbors`.  
- **accuracy_score**: Métrica para calcular a precisão, da biblioteca `sklearn.metrics`.  

---

## ⚠️ **Atenções**  
- Certifique-se de que as variáveis `x_treino`, `x_teste`, `y_treino` e `y_teste` estejam corretamente definidas.  
- Verifique a qualidade do conjunto de dados para evitar viés ou inconsistências.  

---

