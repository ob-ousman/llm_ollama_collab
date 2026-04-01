# LLM Open-Source Gratuit avec Google Colab (Ollama + GPU T4)

Ce notebook permet de **lancer gratuitement un LLM open-source dans Google Colab** avec :

* Accélération **GPU T4**
* **Streaming temps réel**
* **Warmup automatique**
* **Changement de modèle facile**
* **Benchmark multi-modèles (optionnel)**

Le tout sans installation locale.

---

# Objectif

Ce notebook démarre automatiquement :

* Un **serveur Ollama**
* Un **modèle open-source**
* Une **API locale**
* Un **chat streaming performant**

Idéal pour :

* Tests rapides de LLM
* Prototypage IA
* Expérimentation multi-modèles
* Développement agents IA
* Data science & ML engineering

---

# Modèles supportés

Le notebook permet d'utiliser facilement plusieurs modèles :

Exemples :

* Llama 3
* Mistral
* Phi-3
* Gemma
* Qwen
* DeepSeek
* TinyLlama

Tu peux en ajouter facilement dans la **Cellule 0**.

---

# Prérequis

1. Ouvrir Google Colab
2. Charger le notebook
3. Activer le GPU

### Activer le GPU

Dans Google Colab :

```
Exécution → Modifier le type d'exécution → GPU → T4
```

Puis cliquer sur **Enregistrer**

---

# Lancement rapide

Exécuter les cellules dans l'ordre :

### 1. Configuration du modèle

Cellule 0 :

Choisir le modèle :

```python
MODEL = "mistral"
```

---

### 2. Vérification GPU

Cellule 1 :

Vérifie que le GPU T4 est bien disponible

---

### 3. Installation Ollama

Cellule 2 :

Installe automatiquement :

* Ollama
* dépendances système
* utilitaires

---

### 4. Démarrage serveur Ollama

Cellule 3 :

* Lance le serveur Ollama
* Configure GPU
* Optimise performances

---

### 5. Téléchargement du modèle

Cellule 4 :

* Télécharge le modèle
* Warmup automatique
* Précharge en VRAM

---

### 6. Test + Streaming

Cellule 5 :

* Test complet
* Streaming tokens
* Benchmark performance

---

### 7. Benchmark multi-modèles (Optionnel)

Cellule 6 :

Compare plusieurs modèles :

* vitesse
* latence
* qualité réponse

---

# Changer de modèle

Modifier uniquement la **Cellule 0**

Exemple :

```python
MODEL = "llama3"
```

Puis relancer :

```
Runtime → Restart & Run All
```

---

# Performance attendue (GPU T4)

Approximation :

| Modèle     | VRAM | Vitesse |
| ---------- | ---- | ------- |
| TinyLlama  | ~2GB | ++++    |
| Phi-3 mini | ~4GB | +++     |
| Mistral 7B | ~6GB | ++      |
| Llama 3 8B | ~7GB | +       |

---

# Exemple d'utilisation

```python
chat_stream([
    {"role": "user", "content": "Explique moi le machine learning simplement"}
])
```

---

# Architecture

```
Google Colab
     ↓
GPU T4
     ↓
Ollama Server
     ↓
LLM Open-Source
     ↓
API REST locale
     ↓
Streaming réponse
```

---

# Cas d'usage

* Agents IA
* Chatbots
* RAG
* Fine-tuning tests
* Data analysis
* Prompt engineering
* Multi-agents

---

# Limitations Google Colab Gratuit

* Session limitée (~12h)
* GPU partagé
* RAM limitée

Mais largement suffisant pour :

* tests
* prototypage
* démonstration

---

# Avantages

✅ Gratuit
✅ GPU inclus
✅ Aucun setup local
✅ Multi-modèles
✅ Streaming
✅ API locale

---

# Fichier Notebook

```
llm_server_ollama_multi_models.ipynb
```

---

# Astuce

Pour de meilleures performances :

* Utiliser **GPU T4**
* Privilégier modèles 7B ou moins
* Activer warmup

---

# Ready

Tu peux maintenant lancer ton LLM open-source gratuitement dans Google Colab.
