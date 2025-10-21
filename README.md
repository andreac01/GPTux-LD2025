# Addestra il tuo GPTux - Linux Day 2025

Questo repository contiene il materiale per il corso "Addestra il tuo GPTux", presentato al Linux Day 2025. Il corso guida passo-passo nella costruzione, esplorazione e addestramento di un piccolo modello Transformer (GPTux) usando strumenti **open source**.

## Contenuto del corso

- **Introduzione ai Transformer e GPT**: Cos'è un Transformer, come funziona l'attenzione, tokenizzazione, embedding, layer norm, MLP.
- **Notebook interattivo**: Il file [`GPTux.ipynb`](GPTux.ipynb) contiene codice e spiegazioni per:
  - Analizzare la tokenizzazione e la struttura dei dati testuali.
  - Esplorare i componenti fondamentali di un modello GPT (embedding, attenzione, MLP, layer norm).
  - Caricare e confrontare un modello pre-addestrato open source (Pythia/GPT-NeoX).
  - Eseguire un mini-training su un esempio.
  - Visualizzare i risultati e capire come funziona la generazione di testo.

## Setup su Linux (consigliato)

Per un'esperienza completa e locale, si consiglia di utilizzare **Jupyter Notebook** in un ambiente virtuale Python. Tutti i tool utilizzati sono **open source**.

### 1. Installa Python (testato su 3.11 e 3.13)

Assicurati di avere Python installato. Puoi verificarlo con:

```sh
python3 --version
```

Se non è installato, puoi installarlo tramite il gestore pacchetti della tua distribuzione (ad esempio su Ubuntu):

```sh
sudo apt update
sudo apt install python3 python3-venv python3-pip
```

### 2. Crea un ambiente virtuale

```sh
python3 -m venv gptux-env
source gptux-env/bin/activate
```

### 3. Installa i pacchetti necessari

```sh
pip install --upgrade pip
pip install -r requirements.txt
pip install jupyter
```

### 4. Avvia Jupyter Notebook

```sh
jupyter notebook
```

Si aprirà una pagina web dove potrai selezionare e modificare il notebook [`GPTux.ipynb`](GPTux.ipynb).

### Risorse utili

- [Guida ufficiale Jupyter Notebook](https://jupyter.org/)
- [Python e Virtual Environments](https://wiki.archlinux.org/title/Python/Virtual_environment)
- [Jupyter Notebook Install](https://docs.jupyter.org/en/stable/install.html)

## Alternative: Google Colab / Kaggle

Se preferisci non installare nulla in locale, puoi caricare il notebook su [Kaggle Notebooks](https://www.kaggle.com/code) o [Google Colab](https://colab.research.google.com/). Queste piattaforme offrono ambienti preconfigurati e GPU gratuite, ma **la soluzione consigliata rimane quella locale** per promuovere l'uso di strumenti open source e la piena autonomia.

## Note finali

- Tutto il materiale è pensato per essere **didattico** e modificabile.
- Il materiale è più ampio rispetto a quanto coperto nel corso. Puoi esplorarlo a tuo piacimento.
- Il notebook è auto-contenuto: ogni cella spiega e mostra il funzionamento dei vari componenti di un modello GPT (GPTneoX).
- La licenza del material è [GNU GPL v3](LICENSE).

Buon Linux Day e buon divertimento con il tuo GPTux!
