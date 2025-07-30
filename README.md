#DQN LunarLander

Dieses Projekt zeigt, wie ein Deep Q-Network (DQN) auf die Umgebung 'LunarLander-v2' von OpenAI Gym angewendet wird. Ziel ist es, einen Agenten zu trainieren, der möglichst stabil und sicher landet.

1. Voraussetzungen

Wichtig:
Die Version numpy==1.23.5 ist notwendig, um Fehler mit np.bool zu vermeiden, da neuere Versionen von NumPy nicht mit box2d-py kompatibel sind.

Installation:
Die benötigten Pakete sind in der Datei requirements.txt aufgelistet und können mit folgendem Befehl installiert werden:

    pip install -r requirements.txt

2. Ausführung des Notebooks

Die Datei dqn_lunarlander.ipynb enthält den gesamten Projektablauf:

- Aufbau des neuronalen Netzwerks (Q-Network)
- Training des Agenten mit Replay Buffer und ε-greedy Policy
- Visualisierung des Lernfortschritts
- Testphase mit neuen Episoden
- Erstellung von .gif-Videos auf Basis der trainierten Policy

Das Notebook kann lokal in Jupyter oder in Google Colab ausgeführt werden.
Alle Schritte sind klar kommentiert und laufen nacheinander automatisiert ab.

3. Videoausgabe

Während des Tests werden Videos von vollständigen Episoden aufgenommen und im Ordner videos/ als .gif-Dateien gespeichert.

Der jeweilige Reward (Punktewert) ist im Dateinamen enthalten. Ein hoher Reward (>200) zeigt eine besonders gute Steuerung und Landung.

4. Projektstruktur

├── dqn_lunarlander.ipynb        # Jupyter Notebook mit Training, Test & Visualisierung
├── requirements.txt             # Benötigte Python-Bibliotheken
├── README.txt                   # Diese Datei
└── videos/                      # Beispiel-Videos vom Agenten
    ├── lunarlander_episode_0_reward_143.gif
    └── lunarlander_episode_1_reward_172.gif
