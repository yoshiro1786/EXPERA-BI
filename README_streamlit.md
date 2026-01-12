# Streamlit: Reportes de productos vendidos (upgradedb)

## 1) Crear entorno e instalar deps
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## 2) Variables de entorno
Copia `.env.example` a `.env` y completa credenciales.

Si usas `direnv`:
```bash
cp .env.example .env
set -a; source .env; set +a
```

## 3) Ejecutar
```bash
streamlit run app_streamlit_reportes.py
```

## 4) Conexión por túnel SSH (opcional)
Si en producción prefieres túnel:
```bash
ssh -N -L 5433:localhost:9090 root@TU_IP
```
Y en `.env`:
```
PG_HOST=localhost
PG_PORT=5433
```
