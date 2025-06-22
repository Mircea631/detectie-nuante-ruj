# 💄 Aplicație Streamlit – Recunoaștere Nuanță Ruj Avon (Interfață UI Personalizată)

Această aplicație permite recunoașterea nuanțelor de ruj din imagini prin segmentarea buzelor cu modelul Roboflow, potrivirea culorii dominante cu o bază de date Avon, și afișarea interactivă a rezultatelor direct în interfața web.

## ✨ Funcționalități

- Upload mai multor imagini simultan
- Segmentare buze cu model Roboflow
- Extragerea culorii dominante doar din regiunea buzelor
- Clasificarea nuanței (roșu, nude, prună etc.)
- Sugestie ruj Avon în funcție de potrivirea RGB
- Interfață vizuală îmbunătățită:
  - Secțiuni expandabile pentru fiecare imagine (`st.expander`)
  - Afișare culoare + detalii ruj pe 2 coloane

## 🗂 Fișiere

- `streamlit_app.py` – aplicația principală
- `requirements.txt` – dependențele necesare
- `avon_lipsticks.csv` – fișierul cu nuanțele de ruj Avon

## 🚀 Lansare pe Streamlit Cloud

1. Creează un nou repository GitHub și urcă toate fișierele
2. Mergi la [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Creează o aplicație:
   - Main file path: `streamlit_app.py`
4. Adaugă cheia Roboflow în `Secrets`:

```toml
ROBOFLOW_API_KEY = "cheia_ta_de_la_roboflow"
```

5. Click **Deploy** și încarcă imagini pentru analiză

## 🛠 Rulare locală (alternativ)

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
```

## 🧠 Notă

Pentru a obține o cheie API Roboflow:
- Creează cont gratuit pe [roboflow.com](https://roboflow.com)
- Accesează tabul **Deploy** dintr-un model cu segmentare buze
- Copiază cheia după `Authorization: Bearer ...`

---

© Proiect didactic pentru recunoașterea nuanțelor de ruj – suport licență/masterat

