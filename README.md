
# 🏥 Analisi e Valutazione della Coronary Artery Disease (CAD)

## 📌 Descrizione del Progetto
Questo progetto mira a individuare il miglior modello predittivo per la malattia delle arterie coronarie (CAD) attraverso l'uso di tecniche di **machine learning**. L'analisi si concentra sulla selezione del modello con le migliori metriche di accuratezza e sulla sua interpretabilità mediante il metodo SHAP.

## 📂 Struttura del Progetto
- 📊 **`dataset/`**: Contiene i dati utilizzati per l'analisi.
- 🛠 **`scripts/`**: Include gli script R per la pulizia dei dati, l'analisi esplorativa e la modellazione.
- 📑 **`notebooks/`**: Notebook Jupyter e RMarkdown con analisi dettagliate.
- 📜 **`results/`**: Report e visualizzazioni dei risultati ottenuti.
- 📖 **`README.md`**: Questo file, che fornisce informazioni dettagliate sul progetto.

## 📋 Requisiti
Per eseguire il progetto, assicurati di avere installati i seguenti pacchetti in R:
```r
install.packages(c("tidyverse", "randomForest", "xgboost", "caret", "shap", "ggplot2"))
```

## 🚀 Esecuzione del Progetto
1. **Clonare il repository**:
   ```sh
   git clone https://github.com/tuo-username/nome-repo.git
   cd nome-repo
   ```
2. **Eseguire la pulizia dei dati**:
   ```r
   source("scripts/data_cleaning.R")
   ```
3. **Analisi esplorativa e feature engineering**:
   ```r
   rmarkdown::render("notebooks/EDA_Feature_Engineering.Rmd")
   ```
4. **Allenare i modelli**:
   ```r
   source("scripts/model_training.R")
   ```
5. **Valutare i risultati**:
   ```r
   rmarkdown::render("notebooks/Model_Comparison.Rmd")
   ```

## 📊 Metodologia
1. **🔍 Analisi Esplorativa dei Dati (EDA)**: Esame delle variabili, test statistici e visualizzazioni.
2. **⚙️ Feature Engineering**: Selezione e trasformazione delle feature con **RFE (Recursive Feature Elimination)**.
3. **🧠 Modellazione**: Addestramento e confronto tra:
   - **Regressione Logistica**
   - **KNN (K-Nearest Neighbors)**
   - **Random Forest**
   - **Boosting (XGBoost)**
   - **Reti Neurali**
4. **📈 Interpretabilità**: Analisi con **SHAP (Shapley Additive Explanations)**.
5. **🔬 Confronto Modelli**: Analisi delle performance con metriche come **AUC, precision, recall e F1-score**.

## 📜 Risultati Principali
📌 Il miglior modello selezionato è stato **XGBoost**, che ha mostrato:
- **Accuratezza più elevata rispetto agli altri modelli**
- **Migliore capacità di generalizzazione**
- **Interpretabilità grazie a SHAP**

## 👩‍💻 Autore
**Carmela Pia Senatore**

## ⚖️ Licenza
Questo progetto è rilasciato sotto la licenza MIT.

