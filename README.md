# API de Recomendação Musical (pt-BR)

Endpoints (`GET /`).

## Como rodar
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```
- Home: http://127.0.0.1:8000/
- Docs: http://127.0.0.1:8000/docs

## Endpoints
- `GET /recomendacoes/conteudo/{titulo_musica}?limite=5&pesos={"Energy":2.0}`
- `POST /recomendacoes/genero-artista`
- `GET /recomendacoes/colaborativa/{usuario_id}?limite=5`
- `POST /recomendacoes/hibrida`
- `GET /recomendacoes/populares?ano=2017&genero=Pop&limite=5`
