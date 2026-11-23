# CivicAI

```
civicai/
├── backend/            Python (Flask)
│   ├── app.py          API + serves the frontend
│   ├── schemes.py      scheme catalog (3 languages)
│   ├── requirements.txt
│   └── .env.example    copy to .env and add your NEW Gemini key
└── frontend/           HTML / CSS / JS
    ├── index.html
    ├── css/style.css
    └── js/{i18n.js, app.js}
```

## Run
```bash
cd backend
pip install -r requirements.txt
cp .env.example .env      # then edit .env
python app.py             # open http://127.0.0.1:5000
```

API: `GET /api/schemes`, `POST /api/helpdesk`, `POST /api/verify-documents`.
Never commit `.env`.
