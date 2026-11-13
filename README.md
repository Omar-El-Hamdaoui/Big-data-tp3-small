# TP3 — Small Data : films

Notebook exécuté : [`trending-movies-analysis-up-to-2026_small_data.ipynb`](trending-movies-analysis-up-to-2026_small_data.ipynb). Il contient l’acquisition, l’EDA avec PySpark, le prétraitement, les transformations, les modèles, l’évaluation graphique et l’API locale FastAPI.

## Exécuter

Python 3.12 et Java 21 recommandés. Installer les dépendances et le noyau Jupyter :

```bash
python3 -m venv .venv
.venv/bin/python -m pip install numpy==2.5.4 pandas==2.3.3 scipy==1.18.1 scikit-learn==1.7.2 matplotlib==3.11.2 seaborn==0.13.2 joblib==1.6.0 pyspark==4.2.0 kagglehub==1.0.3 ipykernel==7.4.0 fastapi==0.162.5 uvicorn==0.54.0 httpx==0.28.1
.venv/bin/python -m ipykernel install --user --name tp3-small --display-name 'Python (TP3 Small Data)'
```

Ouvrir le notebook dans Jupyter/VS Code et exécuter les cellules. KaggleHub récupère `sahilk22/trending-movies-analysis-up-to-2026` à la première exécution; une authentification Kaggle peut être nécessaire.

Pour démarrer l’API locale après l’exécution du notebook, lancer dans une nouvelle cellule :

```python
import uvicorn
uvicorn.run(app, host="127.0.0.1", port=8001)
```

Documentation : http://127.0.0.1:8001/docs.

Les données, modèles et fichiers temporaires générés ne sont pas versionnés.
