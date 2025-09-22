Chelsea FC 24/25 Performance Analytics – Power BI Project
1️⃣ Obiettivo del Report

Questo progetto ha due scopi principali:

Analisi sportiva: Monitorare l’andamento del Chelsea FC nella stagione 2024/25, valutando risultati, statistiche di squadra e performance individuali.

Analisi strategica: Fornire uno strumento interattivo che permetta a staff tecnico, analisti e stakeholder di prendere decisioni basate sui dati.

KPI chiave analizzati

Risultati partita (gol fatti/subiti, esito)

Expected Goals (xG) e conversion rate

Assist, tiri in porta, passaggi chiave

Minuti giocati, cartellini, sostituzioni

Punteggi medi e trend per competizione

2️⃣ Dataset Utilizzati

Origine: Dati raccolti da fonti pubbliche su risultati e statistiche della stagione 2024/25 (Premier League, FA Cup, EFL Cup, competizioni europee).
Periodo coperto:Sstagione 2024/25 (aggiornamenti per ogni match).
Formato: file CSV elaborati e importati in Power BI.

Tabelle principali

Matches: Dettagli su ogni incontro (data, avversario, risultato, competizione)

Players: Anagrafica e caratteristiche dei giocatori

PlayerStats: Statistiche individuali per match (gol, assist, tiri, passaggi)

Competitions: Informazioni sui tornei disputati

Calendar: Tabella date per analisi temporali

3️⃣ Modellazione Dati

Schema a stella con tabella fatti PlayerStats e dimensioni Players, Matches, Competitions, Calendar.

Relazioni principali:

PlayerStats[playerId] → Players[playerId]

PlayerStats[matchId] → Matches[matchId]

Matches[competitionId] → Competitions[competitionId]

Trasformazioni in Power Query

Pulizia e normalizzazione dei nomi dei giocatori e competizioni

Conversione date in formato standard

Creazione di colonne calcolate per KPI (xG, goal difference, minutaggio cumulato)

4️⃣ Visualizzazioni Presenti

Overview: Sintesi della stagione (risultati globali, andamento forma)

Match Summary: Dettagli su ogni partita con grafici e KPI principali

Player Stats: Dashboard individuali con performance e trend

Competitions: Confronto tra tornei (Premier League, coppe nazionali, Europa)

Insights avanzati: Distribuzione xG, contributo percentuale dei giocatori, heatmap performance

5️⃣ Come Navigare il Report

Slicer principali: Competizione, avversario, giocatore, mese

Drill-through: Dalla pagina generale ai dettagli su un match o su un giocatore

Tooltip personalizzati: Spiegazioni di KPI come xG, conversion rate, media voto

Pulsanti di navigazione: Accesso rapido alle sezioni (Home, Match, Giocatori, Competizioni)

📌 Note e Limitazioni

I dati potrebbero variare rispetto alle statistiche ufficiali per aggiornamenti live o discrepanze nelle fonti.

Alcune metriche (come gli xG) possono essere stimate in base ai dati disponibili.

Il report è ottimizzato per desktop, ma potrebbe presentare differenze su mobile.

📚 Appendice
Glossario

xG: Expected Goals, probabilità media di segnare da una posizione.

Conversion rate: Percentuale di realizzazione dei tiri in porta.

Goal Difference (GD): Differenza reti.

Assist: Ultimo passaggio che porta al gol.

Fonti

Premier League official stats

FBref / StatsBomb (per xG e advanced stats)

UEFA official website

Transfermarkt (rosa e dati anagrafici)

💻 Autore: Roberto Grassia
📅 Anno: 2025
