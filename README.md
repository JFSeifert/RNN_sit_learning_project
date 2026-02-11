## 🔋 Hlavní Projekt: Predikce Spotřeby Elektřiny

### 📊 Popis Projektu

Predikce spotřeby elektrické energie v ČR na 24-48 hodin dopředu pomocí neuronových sítí.

### 🎯 Cíl

Vytvořit model, který dokáže přesně předpovědět spotřebu elektřiny na základě historických dat a externích faktorů (teplota, den v týdnu, svátky).

### 📁 Data

- **Hlavní zdroj:** Hodinová data spotřeby ČR od [OTE](https://www.ote-cr.cz/) (Operátor trhu s elektřinou)
- **Doplňkové zdroje:**
  - Historická hodinová data o teplotě
  - Data o svátcích a dnech v týdnu (kategoriální proměnné)

### 🛠️ Technologie

- **Předzpracování:** pandas, numpy, časové řady
- **Modelování:** LSTM/GRU neuronové sítě (TensorFlow/Keras)
- **Vizualizace:** matplotlib, seaborn, plotly
- **Metriky:** MAE, RMSE, MAPE

### 📋 Postup Projektu

1. **Stažení a příprava dat**
   - Stažení historických dat z OTE
   - Spojení s daty o teplotě a svátcích
   
2. **Explorační analýza**
   - Vizualizace vzorů ve spotřebě
   - Analýza sezónnosti, trendů
   - Korelace s teplotou
   
3. **Předzpracování dat**
   - Feature engineering (den v týdnu, hodina, je_svátek)
   - Normalizace dat
   - Vytvoření časových oken (lookback)
   
4. **Modelování**
   - Implementace LSTM/GRU architektury
   - Trénování modelu
   - Hyperparameter tuning
   
5. **Vyhodnocení**
   - Testování na validation setu
   - Vizualizace predikce vs. realita
   - Analýza chyb

### 📈 Očekávané Výstupy

- Model s MAPE < 5% na 24h predikcích
- Interaktivní dashboard s vizualizacemi
- Dokumentace celého procesu
