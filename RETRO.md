# Retrospective — Progetto Scuolabus Web

**Data:** 2026-04-15
**Team:** Goksu (PM), Piotr (architecture), Thomas (code)
**Durata:** ~1 giorno

---

## ✅ Cosa è andato bene

1. **Coordinamento PM rapido** — Goksu ha creato ticket, assegnato, e mantenuto visibilità su Linear
2. **Deploy GitHub Pages** — Sito pubblicato e raggiungibile in meno di 2 ore
3. **Token GitHub disponibile** — Accesso diretto ha permesso push immediato
4. **Struttura chiara dei task** — 4 ticket ben definiti (architecture, content, dev, deploy)

---

## ❌ Cosa è andato male

1. **Piotr e Thomas non hanno risposto** — Bot attivi ma senza sessioni attive/funzionanti
2. **Nessun commit dai ragazzi** — Goksu ha dovuto fare tutto il lavoro da sola
3. **Deploy GitHub Pages iniziale fallito** — 404 per 10+ minuti, risolto con switch a branch `gh-pages`
4. **Setup webhook non completato** — Linear-GitHub webhook non configurato correttamente
5. **Standup del mattino senza risposte** — Team non ha partecipato al daily

---

## 🔧 Learnings per il futuro

### Setup Tecnico
- **Linear deve essere collegato a GitHub via webhook** — configurare PRIMA di iniziare
- **GitHub Pages:** usare branch `gh-pages` per deploy legacy (più veloce del workflow)
- **Token GitHub:** salvare in `/workspace/.credentials/github_{name}.key`
- **Repo naming:** stesso nome su Linear e GitHub per chiarezza

### Processo Team
- **Sessioni agent attive** — Verificare che Piotr/Thomas abbiano sessioni running PRIMA di assegnare task
- **Standup:** serve un meccanismo più affidabile per collect updates
- **PM autonomy:** se team non risponde, Goksu procede comunque (come fatto oggi)

### Skills/Tools da creare
1. **`create_project`** — Crea repo GitHub + progetto Linear con stesso nome, configura webhook
2. **`deploy_pages`** — Pusha e attiva GitHub Pages su branch corretto
3. **`standup_collect`** — Collect automatico standup da tutti i membri team
4. **Webhook setup helper** — Guida step-by-step per collegare Linear ↔ GitHub

---

## 📋 Action Items

| Action | Owner | Priority |
|--------|-------|----------|
| Creare skill `create_project` | Goksu | Alta |
| Creare skill `deploy_pages` | Goksu | Alta |
| Verificare sessioni Piotr/Thomas | Nico | Alta |
| Setup webhook Linear-GitHub | Elisa/Piotr | Media |
| Creare PM playbook per standup | Goksu | Media |

---

**Conclusione:** Progetto deliverato. Team collaboration da migliorare. Skills in sviluppo.
