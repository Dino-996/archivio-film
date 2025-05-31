# Sistema di Gestione Prestiti Biblioteca

Applicazione Java per la gestione dei prestiti librari, sviluppata con Vaadin e Spring Boot.

## Funzionalità

### Casi d'Uso Implementati

1. **Caricamento Archivio**
   - Caricamento dati della biblioteca (mock object o file JSON)
   - Per livello intermedio: Caricamento da file JSON selezionato dall'operatore

2. **Ricerca Utenti**
   - Ricerca utenti per nome e/o cognome (entrambi i campi opzionali)
   - Visualizzazione risultati in tabella con:
     - Username, nome, cognome
     - Totale libri presi in prestito
     - Libri attualmente in prestito
   - Risultati ordinati per libri presi in prestito (crescente), poi per libri non restituiti (crescente)

3. **Gestione Prestiti**
   - Selezione utente per visualizzare dettagli
   - Visualizzazione libri raggruppati per autore (ordinati per conteggio decrescente)
   - Aggiunta nuovo prestito (titolo libro, autore, data inizio)
   - Gestione automatica restituzioni se utente ha >3 libri non restituiti
   - Gestione errori per dati non validi

4. **Verifica Archivio**
   - Controllo libri presi in prestito da >6 mesi e non restituiti
   - Verifica che tali libri abbiano autori tutti diversi
   - Visualizzazione risultato verifica

5. **Funzionalità Livello Intermedio**
   - Ricerca autore con durata media prestiti più alta
   - Caricamento archivio da JSON

## Dettagli Tecnici

- **Framework**: Vaadin + Spring Boot
- **Sistema di Build**: Gradle
- **Testing**: JUnit 5
- **Logging**: SLF4J + Logback
- **Lombok**: Per riduzione codice boilerplate

## Dipendenze

- Spring Boot Starter Web
- Vaadin
- SLF4J API
- Logback Classic
- JUnit Jupiter
- Lombok

## Come Eseguire

1. Build con Gradle
2. Avviare applicazione Spring Boot
3. Accedere all'interfaccia su `http://localhost:8080`

## Struttura del Progetto

- `src/main/java`: Codice applicazione (struttura MVC)
- `src/test/java`: Test unitari
- `src/main/resources`: File di configurazione
