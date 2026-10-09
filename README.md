# AEEC · Asistente de Entrevistas Estructuradas por Competencias

Aplicación Streamlit que genera guiones de entrevista estructurada por competencias
(preguntas, repreguntas, indicadores y escala BARS 1-5) a partir de la descripción
de un puesto para Nexalia Logística, S. L. (empresa ficticia del sector privado), con hoja de puntuación ponderada y exportación a Word y CSV.
No evalúa candidatos ni trata datos personales: la valoración es siempre humana.

## Ejecución local
```bash
pip install -r requirements.txt
cp .streamlit/secrets.toml.example .streamlit/secrets.toml   # opcional: añada su clave
streamlit run app.py
```
Sin clave de API la app arranca en **modo demostración**.

## Despliegue en Streamlit Community Cloud
1. Suba `app.py`, `requirements.txt`, `README.md`, `.gitignore` y la carpeta `.streamlit/` (solo el `.example`) a un repositorio de GitHub.
2. En share.streamlit.io: *Create app* → repositorio, rama `main`, archivo `app.py`.
3. En *Advanced settings › Secrets* pegue PROVEEDOR, MODELO y la clave de API.
4. Pulse *Deploy*.
