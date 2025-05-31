# Sistema di Gestione Film Videoteca

Applicazione Java per la gestione di film di una videoteca, sviluppata con Vaadin e Spring Boot.

## Funzionalità

### Casi d'Uso Implementati

1. **Caricamento Archivio**
   - Caricamento dati dell'archivio film (mock object o file JSON)

2. **Ricerca Film**
   - Ricerca film per titolo
   - Visualizzazione risultati in tabella 
   - Risultati ordinati per data di uscita crescente/decrescente

3. **Visualizza Dettagli Film**
   - Selezione film per visualizzare dettagli
   - Visualizzazione attori

4. **Verifica Archivio**
   - Controllo film duplicati
   - Visualizzazione risultato verifica

## Dettagli Tecnici

- **Framework**: Vaadin + Spring Boot
- **Sistema di Build**: Gradle
- **Testing**: JUnit 5
- **Logging**: SLF4J + Logback

## Dipendenze

- Spring Boot Starter Web
- Vaadin
- SLF4J API
- Logback Classic & Core
- JUnit Jupiter

## Come Eseguire

1. Build con Gradle
2. Avviare applicazione Spring Boot
3. Accedere all'interfaccia su `http://localhost:8080`

## Struttura del Progetto

- `src/main/java`: Codice applicazione (struttura MVC)
- `src/test/java`: Test unitari
- `src/main/resources`: File di configurazione
