# Doodle AI

Eine Webapp, in der man im Browser etwas zeichnet und ein selbst trainiertes
neuronales Netz (CNN) errät, was die Zeichnung darstellt. Trainiert wird das
Modell mit dem Google-Datensatz *Quick, Draw!*.

**Status:** 🚧 in Arbeit

## Tech-Stack

- **Machine Learning:** Python, PyTorch, torchvision, NumPy
- **Experimente & Visualisierung:** Jupyter Notebooks, Matplotlib
- **Backend (geplant):** FastAPI
- **Frontend (geplant):** HTML, CSS, JavaScript (Canvas)

## Projektstruktur

```
doodle-ai/
├── backend/          # API-Server (FastAPI, später)
├── frontend/         # Zeichenoberfläche im Browser (HTML/CSS/JS)
├── notebooks/        # Jupyter Notebooks für Datenaufbereitung & Training
├── data/             # Datensatz (nicht im Repo, siehe .gitignore)
├── models/           # Trainierte Modelle (nicht im Repo)
├── requirements.txt  # Python-Abhängigkeiten
├── LICENSE
└── README.md
```

## Setup (Windows / PowerShell)

1. Repository klonen und in den Ordner wechseln:
   ```powershell
   git clone <repo-url>
   cd doodle-ai
   ```
2. Virtuelle Umgebung erstellen:
   ```powershell
   python -m venv .venv
   ```
3. Virtuelle Umgebung aktivieren:
   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```
   Falls PowerShell das Ausführen von Skripten blockiert, einmalig ausführen:
   ```powershell
   Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
   ```
4. Abhängigkeiten installieren:
   ```powershell
   pip install -r requirements.txt
   ```
5. Jupyter starten (optional):
   ```powershell
   jupyter notebook
   ```

## Datensatz & Quellenangabe

Dieses Projekt verwendet den
[Quick, Draw! Datensatz](https://github.com/googlecreativelab/quickdraw-dataset)
von Google, lizenziert unter
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

Die Daten sind nicht Teil dieses Repositorys und müssen separat heruntergeladen werden.

## Lizenz

Der Code dieses Projekts steht unter der [MIT-Lizenz](LICENSE).
