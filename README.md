# LLM Inference Benchmark Dashboard

Dashboard de comparaison de moteurs d'inférence LLM — développé dans le cadre du PFE
2025–2026 chez **Talan Tunisie**, en complément du projet **Adaptive LLM Router**.

🔗 Démo en direct : https://splendid-mochi-a31921.netlify.app

## Contenu

Le dashboard compare **7 moteurs d'inférence** : Ollama, llama.cpp, vLLM, TensorRT-LLM,
SGLang, TGI, LMDeploy — sur des critères mesurés (débit, latence, TTFT, usage GPU/VRAM),
avec des runs mesurés localement (Ollama sur GPU, llama.cpp sur CPU) et des chiffres de
référence issus de la documentation publique des moteurs non testés en local.

Fonctionnalités principales :
- **Overview** — indicateurs clés (moteurs comparés, meilleur débit, latence moyenne, usage GPU)
- **Performance Overview** — graphique comparatif multi-moteurs (débit, TTFT, latence P95, GPU)
- **Real-time Monitor** — suivi en direct des métriques
- **Benchmark Explorer / Engine Comparison / Battle Mode** — exploration et confrontation des moteurs
- **Decision Tree / Simulator** — aide à la décision pour choisir un moteur selon le contexte
- **AI Assistant** — assistant conversationnel pour interroger les résultats de benchmark
- **Reports / References** — export et sources

## Stack technique

Fichier unique `index.html` — HTML/CSS/JS vanilla, graphiques via
[Chart.js](https://www.chartjs.org/) (CDN), police Inter (Google Fonts).
Aucune étape de build : le site se déploie tel quel.

## Lancer en local

Aucune dépendance à installer — ouvre simplement `index.html` dans un navigateur,
ou sers-le avec un petit serveur statique :

```bash
npx serve .
```

## Déployer

Déployé actuellement sur Netlify (glisser-déposer du dossier, ou lié à ce dépôt Git avec
`index.html` à la racine comme point d'entrée — aucune commande de build à configurer).

## Auteurs

Zeyneb Mhedhbi · Maram Laouini — PFE 2025–2026, Talan Tunisie
