# creative-coding
py5 teaching environment

Willkommen! In diesem Repository findest du eine einfache Umgebung, um mit der Python-Bibliothek **py5** zu arbeiten – einer Schnittstelle zu Processing, mit der man kreative Grafiken und Visualisierungen in Python schreiben kann.

Du kannst dieses Projekt direkt im Browser nutzen – **ohne Installation**

---

## 🔗 Loslegen

1. Öffne den folgenden Link:

   👉 **[Notebook im Browser starten](https://mybinder.org/v2/gh/DEIN_USERNAME/py5-binder-template/HEAD?filepath=example.ipynb)**

2. Warte einen Moment, bis die Umgebung geladen ist (kann bis zu 1–2 Minuten dauern).
3. Das Beispiel-Notebook `example.ipynb` öffnet sich automatisch.
4. Du kannst die Zellen bearbeiten und oben mit dem ▶️-Knopf ausführen.

---

## ✏️ Hinweise zur Verwendung

- In Binder kann `py5.run_sketch()` keine interaktiven Fenster öffnen.
- Stattdessen speichern wir die Ergebnisse als Bilddatei mit `py5.save_frame("bild.png")`.
- Die Grafik erscheint dann in der Dateiansicht auf der linken Seite und kann heruntergeladen werden.

---

## 📦 Was ist py5?

**py5** ist eine moderne Python-Alternative zu Processing. Es erlaubt dir, grafische Sketches mit bekannten Konzepten wie `setup()` und `draw()` zu schreiben – aber in reiner Python-Syntax.

Mehr Infos: [https://py5coding.org](https://py5coding.org)

---

## 🧠 Beispiel:

```python
import py5

def setup():
    py5.size(400, 400)
    py5.background(255)
    py5.fill(255, 0, 0)
    py5.ellipse(200, 200, 100, 100)

py5.run_sketch(block=False)
py5.save_frame("mein_kreis.png")
py5.close_sketch()
