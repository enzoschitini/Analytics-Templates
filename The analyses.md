# Analisi dei Dati: Descrittiva, Diagnostica, Predittiva e Prescrittiva

## **1. Analisi Descrittiva**

##### **Obiettivo**:
Rispondere alla domanda: **"Cosa è successo?"**
L'analisi descrittiva si concentra sul riassumere e comprendere i dati disponibili, fornendo una visione chiara delle loro caratteristiche principali.

##### **Metodi e strategie:**
1. **Statistiche descrittive:**
   - **Misure di centralità:** Media, mediana, moda.
   - **Misure di dispersione:** Deviazione standard, varianza, range, IQR (Interquartile Range).
   - **Percentili e quartili:** Per suddividere i dati in intervalli.

2. **Visualizzazioni grafiche:**
   - **Istogrammi:** Per analizzare la distribuzione dei dati.
   - **Boxplot:** Per identificare outlier e osservare la dispersione.
   - **Scatter plot:** Per osservare le relazioni tra due variabili.
   - **Heatmap:** Per rappresentare correlazioni tra variabili numeriche.

3. **Tabelle di frequenza:**
   - Frequenze assolute, relative e cumulative per variabili categoriche.

4. **Matrice di correlazione:**
   - Valuta le relazioni tra variabili numeriche.

##### **Esempi pratici:**
- Analisi delle vendite mensili di un negozio.
- Esplorazione della demografia dei clienti di un servizio.

---

## **2. Analisi Diagnostica**

##### **Obiettivo:**
Rispondere alla domanda: **"Perché è successo?"**
Identifica le cause alla base di determinati eventi o pattern rilevati durante l'analisi descrittiva.

##### **Metodi e strategie:**
1. **Test statistici:**
   - **Test di ipotesi:** t-test, ANOVA (per confrontare gruppi).
   - **Test di correlazione:** Pearson, Spearman, Chi-Square.

2. **Modelli di regressione:**
   - **Regressione lineare:** Per comprendere relazioni lineari tra variabili.
   - **Regressione logistica:** Per predire variabili dipendenti binarie.

3. **Root Cause Analysis (RCA):**
   - **Diagrammi di causa-effetto:** Analisi visiva delle possibili cause (es. diagramma di Ishikawa).
   - **5 Whys:** Tecnica iterativa per risalire alla causa principale.

4. **Feature Importance:**
   - Utilizzo di modelli di machine learning (es. Random Forest) per identificare le variabili più influenti.

5. **Analisi di varianza (ANOVA):**
   - Determina se le differenze tra medie di più gruppi sono statisticamente significative.

##### **Esempi pratici:**
- Identificare le cause del calo delle vendite in un determinato periodo.
- Analizzare le motivazioni per cui certi clienti abbandonano un servizio.

---

## **3. Analisi Predittiva**

##### **Obiettivo:**
Rispondere alla domanda: **"Cosa potrebbe accadere?"**
Utilizza dati storici e algoritmi per prevedere eventi futuri o risultati sconosciuti.

##### **Metodi e strategie:**
1. **Modelli di regressione avanzati:**
   - **Regressione multipla:** Per predire valori continui usando più variabili predittive.
   - **Regressione polinomiale:** Per catturare relazioni non lineari.

2. **Algoritmi di classificazione:**
   - **Random Forest, Gradient Boosting, SVM:** Per classificare risultati in categorie discrete.

3. **Modelli di previsione temporale (Time Series):**
   - **ARIMA, SARIMA:** Per analisi e previsioni di serie temporali.
   - **LSTM (Long Short-Term Memory):** Per catturare dipendenze a lungo termine in dati sequenziali.

4. **Analisi di clustering:**
   - **K-means, DBSCAN:** Per segmentare i dati in gruppi omogenei.

5. **Tecniche di validazione:**
   - **Cross-validation:** Per garantire che i modelli siano robusti e generalizzabili.

##### **Esempi pratici:**
- Prevedere la domanda di prodotti in una catena di distribuzione.
- Stimare il rischio di default di un cliente in ambito finanziario.

---

## **4. Analisi Prescrittiva**

##### **Obiettivo:**
Rispondere alla domanda: **"Cosa dovremmo fare?"**
Fornisce raccomandazioni pratiche e strategie ottimali per azioni future, basandosi su analisi predittive e simulazioni.

##### **Metodi e strategie:**
1. **Ottimizzazione:**
   - **Programmazione lineare/non lineare:** Per ottimizzare risorse o processi.
   - **Algoritmi genetici:** Per risolvere problemi complessi.

2. **Simulazione Monte Carlo:**
   - Testa diversi scenari per valutare rischi e opportunità.

3. **Sistemi di raccomandazione:**
   - **Filtraggio collaborativo o basato sui contenuti:** Per personalizzare suggerimenti o azioni.

4. **Decision Trees avanzati:**
   - Include ponderazioni di rischio e costi per supportare decisioni aziendali.

5. **Scenario Analysis:**
   - Valuta l’impatto di diverse decisioni in base a scenari ipotetici.

6. **Causal Inference:**
   - **A/B testing, Regression Discontinuity:** Per valutare l'efficacia di interventi specifici.

##### **Esempi pratici:**
- Ottimizzare il prezzo dei prodotti per massimizzare i profitti.
- Pianificare la distribuzione delle risorse per ridurre i costi operativi.

---

Ogni tipo di analisi è fondamentale in diverse fasi del processo decisionale. Ad esempio, puoi iniziare con l'analisi descrittiva e diagnostica per comprendere il contesto attuale, passare alla predittiva per prevedere l'impatto di variabili future, e infine usare quella prescrittiva per definire azioni strategiche.