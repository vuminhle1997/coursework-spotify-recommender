# Spotify Recommender System

Dieses Projekt besteht aus zwei Hauptteilen: einem Empfehlungssystem, das auf dem eigenen Hörverlauf basiert, sowie einem Modell, das mit TensorFlow Recommenders (TFRS) entwickelt wurde. Die Daten für den eigenen Hörverlauf wurden von Spotify als JSON-Dateien abgerufen, um die Empfehlungen zu erstellen.

## Dateien im Projekt

### [1.Spotify_Recommenders.ipynb](1.Spotify_Recommenders.ipynb)

In dieser Datei wird ein einfaches Empfehlungssystem erstellt, das auf den eigenen Hörverlauf von Spotify basiert. Die Daten wurden über die Spotify-API abgerufen und im JSON-Format gespeichert. Das Empfehlungssystem nutzt diese Daten, um basierend auf dem individuellen Hörverlauf Empfehlungen zu generieren. Das System baut auf den Attributen der gehörten Tracks auf, um Empfehlungen für neue Musik zu generieren.

### [2.Tensorflow_Recommenders.ipynb](2.Tensorflow_Recommenders.ipynb)

In dieser Datei wird ein weiteres Empfehlungssystem mithilfe von TensorFlow Recommenders (TFRS) entwickelt. TFRS ermöglicht es, Empfehlungsmodelle einfach zu erstellen und zu trainieren. Hier wird eine einfache Implementierung gezeigt, wie man ein Modell trainiert, das auf Nutzerinteraktionen basiert und Empfehlungen für ähnliche Items generiert.

### [requirements.txt](requirements.txt)

Beinhaltet die Notwendigen Bibliotheken, um die Notebooks und Codes auszuführen.

### [Data](/data)

In dem Verzeichnis sind sämtliche Daten meines Hörverlaufes auf Spotify als JSON gespeichert. Diese Dateien werden für zusätzliche Details für die Empfehlungen gefetched.

### [recommender.sql](recommender.sql)

Der SQL-Dump aus der PostgresDB, die für die Empfehlung von Songs notwendig sind. Beinhaltet nur Songs, die ich gehört habe und welche ich selektiert habe.

### Verweise

- Das erste Experiment (`1.Spotify_Recommenders.ipynb`) baut auf eigenen Daten aus dem Spotify-Hörverlauf auf.
- Das zweite Experiment (`2.Tensorflow_Recommenders.ipynb`) zeigt, wie man mithilfe von TensorFlow Recommenders ein Modell zur Empfehlung von Inhalten entwickelt. 

## Installation

Um das Projekt auszuführen, müssen die folgenden Abhängigkeiten installiert werden:

```bash
python3 -m venv $PWD/venv
source venv/bin/activate
pip install -r requirements.txt
```

## Spotify API
Für das Experiment in der Datei 1.Spotify_Recommenders.ipynb wird der Zugriff auf die Spotify API benötigt. Es muss ein Entwicklerkonto erstellt und ein API-Schlüssel erhalten werden, um auf die Daten zugreifen zu können.

## Verwendung
- 1.Spotify_Recommenders.ipynb

Die Spotify-Daten müssen als JSON-Dateien geladen werden, die die richtigen Track-URIs und weitere benötigte Informationen enthalten.

Das Notebook kann gestartet werden, um Empfehlungen basierend auf dem eigenen Spotify-Hörverlauf zu generieren.

Das System filtert bereits gehörte Songs und analysiert Tracks, um Empfehlungen zu erstellen.

- 2.Tensorflow_Recommenders.ipynb

In dieser Datei wird gezeigt, wie TensorFlow Recommenders verwendet werden kann, um ein Modell zu erstellen, das auf Benutzerinteraktionen basiert.

Das Notebook zeigt, wie schnell ein einfaches Empfehlungssystem implementiert werden kann.

Die Verwendung von Machine Learning-Kenntnissen wird empfohlen, um das Modell zu verbessern und weiter anzupassen.

# Zusammenfassung
Das Empfehlungssystem in 1.Spotify_Recommenders.ipynb basiert auf dem eigenen Hörverlauf und generiert Empfehlungen nur basierend auf den gehörten Tracks.

Das TensorFlow-Modell in 2.Tensorflow_Recommenders.ipynb bietet eine skalierbare und benutzerfreundliche Möglichkeit, ein Empfehlungssystem mit TensorFlow Recommenders zu erstellen.

Für fortgeschrittene Empfehlungen können beide Ansätze erweitert und weiter optimiert werden, um individuellere und genauere Empfehlungen zu liefern.
