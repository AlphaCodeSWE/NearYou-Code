# NearYou: Sistema di Notifiche basate sulla Posizione

## Panoramica
NearYou è una piattaforma che offre notifiche personalizzate agli utenti quando si trovano in prossimità di negozi o punti di interesse. Utilizzando tecnologie di streaming dati, database geospaziali e generazione di messaggi con LLM, il sistema crea un'esperienza utente contestuale e personalizzata.

## Caratteristiche Principali
- Tracciamento posizioni in tempo reale con Kafka
- Ricerca geospaziale di negozi vicini con PostgreSQL/PostGIS
- Messaggi personalizzati generati con LLM (via Groq/OpenAI)
- Dashboard utente interattiva con visualizzazione mappa
- Monitoraggio e analisi completi con Grafana e Prometheus

## Installazione e Setup

### Prerequisiti
- Docker e Docker Compose
- Git
- Make (opzionale)

### Installazione Rapida
```bash
# Clona il repository
git clone https://github.com/yourusername/nearyou.git
cd nearyou

# Configura le variabili d'ambiente
cp .env.example .env
# Modifica .env con i tuoi valori

# Avvia i servizi
docker-compose up -d