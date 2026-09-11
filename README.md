# 27-ImportExportSpecialist

App Streamlit de conformité commerciale Royaume-Uni → Maroc (électronique). OCRise deux PDF juridiques (droit d'export UK, droit d'import marocain) via Mistral, traduit le texte marocain en anglais, puis un "Specialist Agent" (utilisant les deux documents comme base de connaissances + recherche DuckDuckGo) produit un rapport de conformité détaillé pour les produits/expéditions saisis ; un "Verification Agent" audite ce rapport, et un "Risk Analysis Agent" évalue les risques légaux, opérationnels et financiers.

## Tech stack

streamlit, agno (Agent, Groq, DuckDuckGoTools), mistralai (OCR), python-dotenv

## Lancer le projet

```bash
pip install -r requirements.txt
```

Créer un `.env` avec `GROQ_API_KEY=...` et `MISTRAL_API_KEY=...`

```bash
streamlit run app.py
```
