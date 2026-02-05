# 🧮 Universal Converter Tool

> Un tool di conversione all-in-one, leggero e moderno, contenuto in un singolo file HTML.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Zero Dependencies](https://img.shields.io/badge/Dependencies-0-success?style=flat-square)

Questo progetto fornisce un'interfaccia web pulita e reattiva per tre delle operazioni di conversione più comuni e spesso tediose per sviluppatori e studenti di informatica. È costruito seguendo gli standard moderni del web (ES6+, CSS Flexbox/Grid), senza alcuna libreria esterna.

---

## 🚀 Funzionalità

### 1. Conversione Basi Numeriche (Radix)
Converti istantaneamente numeri tra qualsiasi base da **2 a 36**.
- **Bidirezionale:** Modifica l'input o l'output e l'altro si aggiorna automaticamente.
- **Supporto completo:** Gestisce Binario, Ottale, Decimale, Esadecimale e basi personalizzate.
- **Validazione:** Previene input non validi per la base selezionata.

### 2. Codifica e Decodifica Testo
Gestione robusta delle stringhe per il web.
- **Plain Text ↔ Base64:** Implementazione sicura per UTF-8 (gestisce correttamente accenti ed emoji, risolvendo il problema classico di `btoa`/`atob`).
- **Plain Text ↔ URL Encoded:** Percent-encoding per parametri web.

### 3. IEEE 754 Floating Point (32-bit)
Visualizza come i numeri decimali sono rappresentati in memoria a livello di bit.
- **Ispezione Bit:** Vedi la rappresentazione binaria esatta di un `float`.
- **Modifica Bit:** Cambia i bit (0/1) e vedi come cambia il numero decimale.
- **Visualizzazione Componenti:** Evidenziazione cromatica di **Segno**, **Esponente** e **Mantissa**.

---

## 🛠 Dettagli Tecnici

Il codice è stato scritto per essere performante e didattico ("State of the Art"):

- **Single File:** Tutto (HTML, CSS, JS) è contenuto in un unico file per la massima portabilità.
- **JavaScript Moderno:**
  - Utilizzo di **`ArrayBuffer`** e **`DataView`** per la manipolazione precisa della memoria nella conversione IEEE 754, evitando calcoli matematici approssimativi.
  - **Event Delegation** e listener ottimizzati.
  - **IIFE** (Immediately Invoked Function Expressions) per incapsulare la logica e non inquinare il global scope.
- **CSS Responsivo:** Layout fluido basato su CSS Variables (`:root`), Flexbox e Grid. Nessun framework CSS pesante (Bootstrap/Tailwind) richiesto.

---

## 📦 Installazione e Utilizzo

Non è richiesta alcuna installazione, build process (Webpack/Vite) o server backend.

1. **Scarica** il file `converter.html`.
2. **Apri** il file con qualsiasi browser web moderno (Chrome, Firefox, Edge, Safari).
3. **Usa** il tool offline o online.

### Esecuzione Rapida
Basta fare doppio click sul file:
```bash
open converter.html
