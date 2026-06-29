Davide Izzo

AI Specialist · Machine Learning & Computer Vision

Sviluppo applicativi e automazioni basati su Machine Learning e Intelligenza Artificiale: dall'addestramento di modelli di deep learning alle pipeline di Computer Vision end-to-end, fino alle web app che integrano modelli di AI e all'analisi e visualizzazione dei dati. Specializzazione AI Specialist (ITS), con esperienza pratica nel mondo dello Sport Analytics e dell'Health-tech.

Mi muovo lungo l'intero ciclo: capire il problema → costruire ed etichettare i dati → addestrare e validare i modelli → integrarli in una pipeline → restituire risultati leggibili e visualizzabili.

📍 Marche, Italia · 💼 Open to work

🔗 [LinkedIn](https://www.linkedin.com/in/davide-izzo-86445b142/) · ✉️ [dizzo20395@gmail.com](mailto:dizzo20395@gmail.com)


🧠 Competenze tecniche

Linguaggi: Python · SQL · JavaScript

Deep Learning: PyTorch · YOLO (v8 / v11) · CNN · Reti Neurali · Transfer Learning · Training & validazione modelli · Dataset building & labeling

Computer Vision: OpenCV · Object Detection · Multi-Object Tracking (OC-SORT, Hungarian, Kalman) · Homography · Camera Calibration · OCR

Machine Learning: Scikit-learn · Regression · Decision Trees · Random Forest · K-Means · PCA · Anomaly Detection · Recommender Systems · Reinforcement Learning

AI Applicata: Integrazione di LLM · NLP · Prompt Engineering · API REST

Sviluppo: Web App · PWA (Progressive Web App) · Streamlit · sviluppo cross-device (desktop & mobile)

Dati & Visualizzazione: Pandas · NumPy · SciPy · Matplotlib · Seaborn · Plotly

Strumenti & Database: Jupyter · Google Colab · VS Code · Git/GitHub · MySQL · SQLite


🚀 Progetti in evidenza

⚽ K-Vision Soccer — Computer Vision per l'analisi di partite di calcio · K-Sport World

Pipeline modulare di Computer Vision che traccia separatamente giocatori, portieri, arbitri e palla da video di partite e ne estrae le metriche di gioco.


Detection con modello YOLOv8 (Large) addestrato da me su 4 classi (portiere, palla, arbitro, giocatore), su GPU NVIDIA A100 ad alta risoluzione (imgsz 3840) — mAP@50 ≈ 0.99 · mAP@50-95 ≈ 0.77 · precision ≈ 0.96 · recall ≈ 0.97
Multi-object tracking dedicato per entità: OC-SORT (giocatori, con NMS + auto-tune), Hungarian Algorithm (arbitri/portieri), Kalman Filter + RTS Smoother (palla)
Omografia duale + undistortion per la conversione pixel → coordinate reali di campo
Metriche cinematiche per individuo (posizione, velocità, distanza) con smoothing fisico (Savitzky-Golay); analisi dei contatti palla
Output pronti per la piattaforma di analisi (.kref / .kball), grafici comparativi e video con mappa tattica animata


Python · YOLOv8 · OpenCV · OC-SORT · Kalman Filter · Homography · NumPy · Pandas


Lavoro professionale (K-Sport World). Demo dimostrativa disponibile su richiesta.



🎾 K-Vision Tennis — Computer Vision per l'analisi di match di tennis · K-Sport World

Sistema di analisi dei match di tennis da broadcast TV, con un'architettura a due domini:


Dominio fisico (CV/GPU): segmentazione automatica degli scambi (rally), detection e tracking dei giocatori, court keypoints, omografia, conversione in metri, derivazione di velocità e distanze
Dominio informativo (OCR): lettura del punteggio, dei nomi e del servizio dal tabellone, con matching su whitelist
Modelli dedicati: yolo11l_players.pt (giocatori) e yolo11m_court.pt (campo)
Modello giocatori addestrato da me (vedi sotto): YOLOv11, mAP@50 ≈ 0.99, mAP@50-95 ≈ 0.87


Python · PyTorch · YOLOv11 · OpenCV · OCR · Multi-Object Tracking · Homography


Lavoro professionale (K-Sport World). Demo dimostrativa disponibile su richiesta.



🧪 Addestramento YOLOv11 — Tennis Player Detection (Deep Learning)

Progetto di deep learning end-to-end per addestrare il modello di detection dei giocatori usato in K-Vision Tennis.


Dataset costruito da zero: ~5.400 immagini etichettate dai broadcast dei 4 tornei del Grande Slam (erba, terra, cemento)
Pipeline completa: download → estrazione frame → pre-labeling automatico → correzione → split stratificato per superficie → training → validazione per superficie
Transfer learning da pesi COCO, YOLOv11 a imgsz=1280, con esperimenti di augmentation
Risultati: mAP@50 ≈ 0.99 · mAP@50-95 ≈ 0.87 · precision/recall ≈ 0.99


Python · PyTorch · Ultralytics YOLOv11 · yt-dlp · OpenCV · Data Labeling

🩸 Health Analyzer — App AI per la lettura delle analisi del sangue

Progressive Web App (desktop & mobile) che usa un LLM per leggere un referto di analisi del sangue e raggruppare automaticamente i valori per categoria, li salva in un database locale e ne mostra gli andamenti nel tempo. Privacy by design: nessun dato sanitario lascia il dispositivo.

JavaScript · PWA · Service Worker · SQL · Integrazione LLM · HTML/CSS


Progetto personale. In fase di pubblicazione come repository pubblico.



📧 Assistente Email AI

Web app per la generazione e il perfezionamento di email tramite NLP, costruita con Python e Streamlit su API Google Gemini.

Python · Streamlit · NLP · API REST

👁️ Analizzatore di Immagini AI

Strumento di Computer Vision per l'analisi multimodale di immagini: estrazione di dati strutturati (OCR, oggetti, descrizioni).

Python · Computer Vision · OCR · Multimodal AI


🎓 Formazione & Certificazioni


Diploma di Specializzazione Tecnica Superiore (5 EQF) — AI Specialist · ITS Cultura Turismo e Nuove Tecnologie Marche ·  (2024–2026)
Machine Learning Specialization (Supervised ML · Advanced Learning Algorithms · Unsupervised, Recommenders & RL) · Stanford University & DeepLearning.AI — Coursera · 2025
ICDL Essentials · AICA



🌐 Lingue

Italiano (madrelingua) · Inglese (B1) · Francese (B1)


📫 Contatti

[LinkedIn](https://www.linkedin.com/in/davide-izzo-86445b142/) · [dizzo20395@gmail.com](mailto:dizzo20395@gmail.com)
