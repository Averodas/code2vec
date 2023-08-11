# Anleitung Installation code2vec für Regel `PredictMethodNames` für Unix basiertes OS

## Voraussetzungen

geclontes jlint  
Installiertes Python3.6  
(im Folgenden wird vom Installationsort `/usr/bin/python3.6` ausgegangen)

### Schritt 1

In der Konsole in das `jlint` Verzeichnis navigieren.

### Schritt 2

```
cd ..
```

### Angepasstes Code2Vec in paralleles Verzeichnis zu jlint clonen

```
git clone git@github.com:Averodas/code2vec.git
```

### In das Verzeichnis wechseln

```
cd code2vec
```

### Trainiertes Model herunterladen

```
wget https://s3.amazonaws.com/code2vec/model/java14m_model.tar.gz
```

### Model entpacken

```
tar -xvzf java14m_model.tar.gz
```

### Gepacktes Model (~1,5GB) löschen _optional_

```
rm java14m_model.tar.gz
```

### venv erzeugen

```
/usr/bin/python3.6 -m venv .venv
```

### Pip im venv aktualisieren

```
.venv/bin/python3.6 -m pip install --upgrade pip
```

### Tensorflow im venv installieren

```
.venv/bin/python3.6 -m pip install tensorflow==2.0.0
```

## Links

[Angepasstes Code2Vec](https://github.com/Averodas/code2vec)
