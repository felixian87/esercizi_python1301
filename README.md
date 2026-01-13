# 📚 Gestione Voti - Procedura Guidata

Applicazione grafica per la gestione dei voti degli alunni con procedura guidata passo-passo.

## 🎯 Caratteristiche

- **Procedura Guidata**: 4 step per configurare tutto prima di inserire i voti
  1. Schermata di benvenuto
  2. Aggiunta alunni
  3. Aggiunta materie
  4. Inserimento voti
- **Salvataggio automatico** in formato JSON
- **Visualizzazione voti** con statistiche dettagliate
- **Interfaccia moderna** e intuitiva
- **Eseguibile standalone** (.exe)

## 📋 Requisiti

- Python 3.9+ (solo per lo sviluppo)
- Windows (per l'eseguibile .exe)

## 🚀 Come usare

### Opzione 1: Eseguibile .exe (Consigliato)

1. Scarica `Gestione_Voti.exe` dalla cartella `dist/`
2. Doppio click per avviare
3. Non servono altri file!

### Opzione 2: Esecuzione da Python

```bash
python gestione_voti_app.py
```

## 🔨 Creazione dell'eseguibile

### Metodo 1: Script Python

```bash
python build_exe.py
```

### Metodo 2: Script Batch

```batch
crea_exe.bat
```

Questo creerà il file `Gestione_Voti.exe` nella cartella principale.

## 📁 File generati

Quando usi l'applicazione, viene creato:

- **voti.json**: Contiene tutti i voti salvati

```json
{
  "Mario Rossi": {
    "Matematica": [8.5, 9.0, 7.5],
    "Italiano": [8.0, 9.5]
  },
  "Anna Bianchi": {
    "Matematica": [9.0, 9.5],
    "Italiano": [8.5, 8.0]
  }
}
```

## 📊 Step della Procedura

### Step 1: Aggiungi Alunni
- Inserisci i nomi degli alunni uno per uno
- Puoi rimuovere alunni prima di continuare

### Step 2: Aggiungi Materie
- Inserisci le materie che insegni
- Puoi rimuovere materie prima di continuare

### Step 3: Inserisci Voti
- Seleziona alunno e materia dai menu dropdown
- Inserisci il voto (0-10)
- I voti vengono aggiunti in tempo reale

### Step 4: Visualizzazione e Statistiche
- Visualizza tutti i voti registrati
- Vedi le medie per ogni materia
- Consulta le statistiche generali (media classe, min/max)

## 💾 Caricamento dati precedenti

Alla prima schermata puoi scegliere:
- **Nuovo Progetto**: Crea un nuovo set di dati
- **Carica Dati**: Carica i voti salvati precedentemente da `voti.json`

## 🎨 Interfaccia

- Design moderno con tema scuro
- Pulsanti colorati e intuitivi
- Icone emoji per migliore leggibilità
- Finestra ridimensionabile

## ⚙️ Configurazione per la distribuzione

Se vuoi distribuire l'eseguibile:

1. Assicurati che `gestione_voti_app.py` sia aggiornato
2. Esegui `python build_exe.py`
3. Il file `Gestione_Voti.exe` sarà pronto nella cartella principale
4. Puoi distribuire solo il `.exe` - non servono altri file!

## 📝 Note tecniche

- L'app usa tkinter (incluso in Python)
- I dati sono salvati in JSON per facile accesso e modifica
- L'eseguibile è a singolo file (--onefile)
- Nessun file di configurazione necessario

## 🤝 Supporto

Per problemi o suggerimenti, controlla:
- Che `voti.json` abbia permessi di scrittura
- Che Python sia aggiornato
- I log di PyInstaller se l'exe non si crea

---

**Versione**: 1.0.0
**Data**: Gennaio 2026
