# 🎛️ Maschera Regia OBS – Puccia Linux

Questa cartella contiene la **maschera regia** per gestire la proiezione e la scaletta degli interventi al **Puccia Linux**, pensata per l'uso con **OBS Studio**.

> ✅ Timer visivo, suoni inclusi, maschera proiettabile e pronta all’uso!

---

## 📂 Contenuto

- `timer.html` – Timer ciclico con fasi **Talk (15 min)** e **Pausa (2 min)**
- `elevator.wav` – Musica da ascensore (loop durante la pausa)
- `gong.wav` – Suono di **campanella** al cambio fase
- `Maschera_Regia_OBS.json` – Collezione di scena OBS esportata
- `README.md` – Questo file

---

## 🕒 Come funziona il timer

1. Parte automaticamente con 15 minuti di **Talk**
   - Il testo cambia colore dal **verde al rosso** in transizione
   - Allo scadere: **suona una campanella**
2. Inizia automaticamente una **pausa di 2 minuti**
   - Parte musica da ascensore in **loop**
3. Il ciclo riparte in automatico
4. Include un pulsante **"Riavvia Timer"** per ricominciare in qualsiasi momento

---

## 🔧 Come usare con OBS Studio

### ▶️ Metodo consigliato:

1. Aggiungi una **Browser Source** in OBS
2. Inserisci come URL:
   ```
   file:///percorso/assoluto/del/file/timer.html
   ```
   Esempio:
   ```
   file:///C:/Users/TuoNome/Desktop/Maschera_Regia_Obs/timer.html
   ```
3. Imposta dimensioni (es. 1920x1080)
4. Usa la scena come sfondo visivo per la regia

---

## 🔁 Alternativa: Importare la collezione OBS

Puoi importare la collezione `Maschera_Regia_OBS.json` per avere subito pronta la scena:

- In OBS → **File → Collezioni di scene → Importa**
- Seleziona il file `Maschera_Regia_OBS.json`
- Verifica che le sorgenti locali (immagini, timer.html, audio) siano correttamente collegate

### 📺 Scene e sorgenti configurate:
- Scena principale: `Puccia_Live`
- Sorgenti incluse:
  - **Immagine**: sfondo (`lavagna.jpg`)
  - **Browser**: `timer.html` in locale
  - **Cattura schermo (PipeWire)`**: per proiettare eventuali contenuti dal desktop
- Transizione attiva: **Dissolvenza** (300ms)

---

## 🧰 Requisiti

- OBS Studio (v29 o superiore consigliato)
- Browser moderno (per aprire `timer.html` anche fuori da OBS)
- Supporto audio `.wav` abilitato nel browser o in OBS
- File `lavagna.jpg` presente nel percorso previsto, oppure da riconfigurare

---

## 📄 Licenza

Questa maschera è rilasciata sotto licenza **CC BY-SA 4.0**.  
Può essere modificata, adattata e riutilizzata citando la fonte.

---

## 🙌 Autori

Realizzata da William e il team **Puccia Linux**  
Contributi e modifiche sono benvenuti!

