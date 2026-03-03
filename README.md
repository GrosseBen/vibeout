# VibeOut

**Think. Link. Decide. Code. Build.**

🔥 **Dein Second Brain als Code** – Diskussionen, Entscheidungen und Wissensmanagement **vollautomatisiert** mit Mistral Vibe + Go.

[MIT License](LICENSE)  
[Docker Ready](https://github.com/GrosseBen/vibeout/pkgs/container/vibeout)

---

## 🌟 Vision

VibeOut kombiniert **Mistral Vibe** (für natürliche Diskussionen) mit **Go-Mikroservices** (für Performance) und **Docker** (für Portabilität).  
**Ziel**: Ein **selbstpflegendes Wissenssystem**, das:

- **Diskussionen** in Echtzeit dokumentiert (`vibeout/think`).
- **Entscheidungen** als arc42-ADRs speichert (`vibeout/decide`).
- **Wissen vernetzt** (automatische `[[Links]]` + Mermaid-Graphen).
- **Podcasts generiert** (aus Diskussionen → MP3 mit KI-Stimmen).

**Für wen?**  
Developern, Architekten und Teams, die **keine Zeit für manuelles Dokumentieren** haben.

---

## 🚀 Schnellstart (Docker)

```bash
# 1. Repo klonen
git clone https://github.com/GrosseBen/vibeout
cd vibeout

# 2. Docker starten (Go-Server + Vibe)
docker-compose up -d

# 3. Diskussion beginnen
docker-compose exec vibe vibe --agent vibeout/think
> was bisher geschah diskussionen/beispiel.md
```

*(Hinweis: Docker-Images folgen in Kürze!)*

---

## 🗺 Roadmap


| Phase          | Features                                                  | Status               |
| -------------- | --------------------------------------------------------- | -------------------- |
| **🟢 Phase 1** | Basis-Skills (`think`, `decide`), lokale Dateispeicherung | **Aktiv**            |
| **🟡 Phase 2** | Go-MCP-Server (für Performance), Docker-Integration       | **Nächste Schritte** |
| **🔴 Phase 3** | Podcast-Generierung, GitHub-Integration, Obsidian-Sync    | **Geplant**          |


**Mithelfen?**  
[Issues](https://github.com/GrosseBen/vibeout/issues) öffnen oder Pull Requests einreichen!

---

## 📂 Struktur

```
vibeout/
├── docker/          # Docker-Compose für Go-Server + Vibe
├── skills/          # Vibe-Skills (z. B. `think/`, `decide/`)
├── mcp-server/      # Go-Backend für komplexe Logik
└── data/            # Persistente Daten (Diskussionen, Git-Repos)
```

---

## 🛠 Technologien


| Komponente     | Technologie     | Zweck                      |
| -------------- | --------------- | -------------------------- |
| **Skills**     | Mistral Vibe    | Natürliche Diskussionen    |
| **Backend**    | Go (MCP-Server) | Schnelle Analysen          |
| **Deployment** | Docker          | Portabel & skalierbar      |
| **Daten**      | Markdown + Git  | Versioniert & durchsuchbar |


---

## 📄 Lizenz

**MIT** – Nutze, modifiziere und teile VibeOut frei!  
*(Siehe [LICENSE](LICENSE) für Details.)*

---

## 🎤 Podcast-Integration

VibeOut kann **Diskussionen automatisch als Podcast-Folgen** exportieren:

- **Stimmen**: ElevenLabs (KI) oder lokale TTS (Piper).
- **Format**: MP3 mit Kapiteln (für YouTube/Spotify).
- **Beispiel**:
  ```plaintext
  > vibeout/podcast "Episode 1: KI-Integration"
  🤖 Output: data/podcasts/episode1.mp3
  ```

*(Demo-Folge folgt!)*

---

## 🤝 Community

- **Discord**: [Link folgt]()
- **E-Mail**: [vibeout@grossesippe.de](mailto:vibeout@grossesippe.de)

---

**„Was bisher geschah… und jetzt: Ahhhh – die Challenge lösen!“** 😉
