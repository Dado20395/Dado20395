# Davide Izzo

### Specialista in IA · Apprendimento automatico e visione artificiale

Sviluppo applicativi e automazioni basate su Machine Learning e Intelligenza Artificiale: dall'addestramento di modelli di deep learning alle pipeline di Computer Vision end-to-end, fino alle web app che integrano modelli di AI e all'analisi e visualizzazione dei dati. Specializzazione AI Specialist (ITS), con esperienza pratica nel mondo dello Sport Analytics e dell'Health-tech — il mio interesse resta l'AI applicata in generale, ovunque possa semplificare un problema reale.

Mi muovo lungo l'intero ciclo: capire il problema → costruire ed etichettare i dati → addestrare e validare i modelli → integrarli in una pipeline → restituire risultati leggibili e visualizzabili.

📍 Marche, Italia · 💼 Disponibile a lavorare
🔗 [LinkedIn](https://www.linkedin.com/in/davide-izzo-86445b142/) · ✉️ [dizzo20395@gmail.com](mailto:dizzo20395@gmail.com)

---

## 🧠 Competenze tecniche

**Linguaggi:** Python · SQL · JavaScript

**Apprendimento profondo:** PyTorch · YOLO (v8 / v11 / 26) · CNN · Reti neurali · Transfer Learning · Training & validazione del modello · Dataset building & labeling

**Visione artificiale:** OpenCV · Rilevamento di oggetti · Tracciamento di oggetti multipli (OC-SORT, ungherese, Kalman) · Omografia · Calibrazione della telecamera · OCR

**Apprendimento automatico:** Scikit-learn · Regressione · Alberi decisionali · Random Forest · K-Means · PCA · Rilevamento delle anomalie · Sistemi di raccomandazione · Apprendimento per rinforzo

**AI Applicata:** Integrazione di LLM · NLP · Prompt Engineering · API REST

**Sviluppo:** Web App · PWA (Progressive Web App) · Streamlit · sviluppo cross-device (desktop & mobile)

**Dati e Visualizzazione:** Pandas · NumPy · SciPy · Matplotlib · Seaborn · Plotly

**Strumenti e database:** Jupyter · Google Colab · VS Code · Git/GitHub · MySQL · SQLite

---

## 🚀 Progetti in corso

### ⚽ K-Vision Soccer — Computer Vision per l'analisi delle partite di calcio · K-Sport World

Pipeline modulare di Computer Vision che traccia separatamente giocatori, portieri, arbitri e palla da video di partite e ne estrae le metriche di gioco.

- Rilevamento con modello YOLOv8 (Large) addestrato da me su 4 classi (portiere, palla, arbitro, giocatore), su GPU NVIDIA A100 ad alta risoluzione (imgsz 3840) — mAP@50 ≈ 0.99 · mAP@50-95 ≈ 0.77 · precisione ≈ 0.96 · richiamo ≈ 0.97
- Tracciamento multi-oggetto dedicato per entità: OC-SORT (giocatori, con NMS + auto-tune), Algoritmo ungherese (arbitri/portieri), Filtro Kalman + RTS Smoother (palla)
- Omografia duale + undistortion per la conversione pixel → coordinate reali di campo
- Metriche cinematiche per individuo (posizione, velocità, distanza) con smoothing fisico (Savitzky-Golay); analisi dei contatti palla
- Output pronti per la piattaforma di analisi (.kref / .kball), grafici comparativi e video con mappa tattica animata

`Python` · `YOLOv8` · `OpenCV` · `OC-SORT` · `Filtro di Kalman` · `Omografia` · `NumPy` · `Pandas`

*Lavoro professionale (K-Sport World). Demo dimostrativa disponibile su richiesta.*

### 🎾 K-Vision Tennis — Computer Vision per l'analisi delle partite di tennis · K-Sport World

Sistema di analisi dei match di tennis da broadcast TV, con un'architettura a due domini:

- **Dominio fisico (CV/GPU):** segmentazione automatica degli scambi (rally), rilevazione e tracking dei giocatori, court keypoints, omografia, conversione in metri, derivazione di velocità e distanze
- **Dominio informativo (OCR):** lettura del punteggio, dei nomi e del servizio dal tabellone, con corrispondenza su whitelist
- Modelli dedicati: `yolo11l_players.pt` (giocatori) e `yolo11m_court.pt` (campo). Modello giocatori addestrato da me: YOLOv11, mAP@50 ≈ 0.99 · mAP@50-95 ≈ 0.87
- Migrazione in corso verso modelli di nuova generazione (YOLO26), con validazione A/B sistematica prima di ogni promozione in produzione

`Python` · `PyTorch` · `YOLOv11` · `YOLO26` · `OpenCV` · `OCR` · `Tracciamento multi-oggetto` · `Omografia`

*Lavoro professionale (K-Sport World). Demo dimostrativa disponibile su richiesta.*

### 🧪 Addestramento YOLOv11 — Tennis Player Detection (Deep Learning)

Progetto di deep learning end-to-end per addestrare il modello di rilevamento dei giocatori usato in K-Vision Tennis.

- Dataset costruito da zero: ~5.400 immagini etichettate dai broadcast dei 4 tornei del Grande Slam (erba, terra, cemento)
- Pipeline completa: download → estrazione frame → pre-labeling automatico → correzione → split stratificato per superficie → training → validazione per superficie
- Transfer learning da pesi COCO, YOLOv11 a imgsz=1280, con esperimenti di augmentation
- Risultati: mAP@50 ≈ 0.99 · mAP@50-95 ≈ 0.87 · precisione/richiamo ≈ 0.99

`Python` · `PyTorch` · `Ultralytics YOLOv11` · `yt-dlp` · `OpenCV` · `Etichettatura dei dati`

### 🩸 Health Analyser — App AI per la lettura delle analisi di laboratorio

Progressive Web App (desktop & mobile) che usa un LLM (Claude) per leggere i referti di laboratorio (sangue, urine, feci), estrarne i valori, classificarli rispetto ai range di riferimento (anche i risultati non numerici) e seguirne gli andamenti nel tempo, con indici derivati e commenti educativi. Privacy by design: nessun dato sanitario lascia il dispositivo.

`JavaScript` · `PWA` · `Service Worker` · `SQL` · `Integrazione LLM (Claude)` · `HTML/CSS`

*Progetto personale. In fase di pubblicazione come repository pubblico.*

### 📧 Assistente email AI

Web app per la generazione e il perfezionamento di email tramite NLP, costruita con Python e Streamlit su API Google Gemini.

`Python` · `Streamlit` · `Elaborazione del linguaggio naturale` · `API REST`

### 👁️ Analizzatore di Immagini AI

Strumento di Computer Vision per l'analisi multimodale di immagini: estrazione di dati strutturati (OCR, oggetti, descrizioni).

`Python` · `Visione artificiale` · `OCR` · `Intelligenza artificiale multimodale`

---

## 🎓 Formazione e Certificazioni

- **Diploma di Specializzazione Tecnica Superiore (5° livello EQF) — Artificial Intelligence Specialist (AI Specialist)**
  Qualifica rilasciata: **Tecnico Superiore Data Manager** · ITS Turismo Marche · 2024–2026
- Machine Learning Specialization (Supervised ML · Advanced Learning Algorithms · Unsupervised, Recommenders & RL) · Stanford University & DeepLearning.AI — Coursera · 2025
- ICDL Essentials · AICA

---

## 🌐 Lingue

Italiano (madrelingua) · Inglese (B1) · Francese (B1)

---

## 📫 Contatti

[LinkedIn](https://www.linkedin.com/in/davide-izzo-86445b142/) · [dizzo20395@gmail.com](mailto:dizzo20395@gmail.com)
