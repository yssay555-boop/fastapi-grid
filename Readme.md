## fastapi 서버 기동
python -m venv venv
venv/Scripts/Activate
pip install -r requirements.txt
uvicorn main:app --reload --host 0.0.0.0 --port 8000

## static html web server live server or 
python -m http.server 8001

## allow_origins=["http://127.0.0.1:8001","http://localhost:8001"],  수정후 API 서버 재기동
### ✅ 이 Origin만 허용 테스트

## API Doc
Swagger UI: http://127.0.0.1:8000/docs
OpenAPI JSON: http://127.0.0.1:8000/openapi.json