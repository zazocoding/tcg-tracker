# Pokémon TCG Collection Tracker

A simple web app to track a personal Pokémon TCG collection, built with Firebase and vanilla JavaScript.

This project can be used as a **template to build your own TCG tracker** (Pokémon, Magic, etc.) but its made to use the .csv file with all the Pokemon up to the nineth generation.

![Architecture Diagram](./assets/example.png)

---

## Features

- Total collection progress
- Progress by generation
- Full collection table
- Add / remove cards from collection
- Binder organization (page & slot tracking)
- Real-time sync with Firebase Firestore

---

##  Tech Stack

- **Frontend**: HTML, CSS, JavaScript (Vanilla)
- **Backend**: Firebase
  - Firestore (database)
  - Firebase Hosting (deployment)
- **Data management**: Python scripts (CSV → Firestore)

---

##  How It Works

Each Pokémon is stored as a document in Firestore:

```json
{
  "dex": "1",
  "name": "Bulbasaur",
  "gen": "Gen 1",
  "owned": true,
  "binderPage": 1,
  "binderSlot": 1
}

