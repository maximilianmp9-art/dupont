# 📊 Modelo DuPont en Streamlit

Esta aplicación desarrollada en **Python** con **Streamlit** permite analizar la rentabilidad de negocios a través del **modelo DuPont**. Está diseñada para aceptar archivos de bases de datos en formato Excel o CSV y genera un reporte interactivo con múltiples indicadores financieros clave.

---

## 🚀 Funcionalidades

- ✅ Carga de archivos `.csv` o `.xlsx`
- 📈 Análisis automático de los siguientes indicadores por período:
  - Margen Neto (%)
  - Rotación de Activos (veces)
  - Apalancamiento (veces)
  - **ROE** (%) = Margen × Rotación × Apalancamiento
  - **ROA** (%) = Rotación × Apalancamiento
  - Pay Back Capital (veces) = 1 / ROE
  - Pay Back Activos (veces) = 1 / ROA
- 📅 Soporta múltiples períodos dinámicamente
- 📥 Descarga del reporte generado en Excel

---

## 📁 Formato del archivo de entrada

El archivo debe tener los siguientes encabezados en las primeras filas:

| Periodo | Ventas Netas | Utilidad Neta | Activos Totales | Capital Contable |
|---------|---------------|----------------|------------------|-------------------|
| 2021    | 1000000       | 100000         | 500000           | 250000            |
| 2022    | 1200000       | 150000         | 600000           | 300000            |
| ...     | ...           | ...            | ...              | ...               |

Puedes cargarlo como `.csv` o `.xlsx`.

---

## 💻 ¿Cómo ejecutarlo localmente?

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tuusuario/tu-repositorio.git
   cd tu-repositorio
   ```

2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

3. Ejecuta la app:
   ```bash
   streamlit run app.py
   ```

---

## ☁️ ¿Cómo desplegarlo en Streamlit Cloud?

1. Sube este repositorio a tu cuenta de GitHub.
2. Ve a [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Selecciona “New App”.
4. Conecta tu repositorio.
5. Elige el archivo `app.py` como punto de entrada.
6. ¡Listo! Tu aplicación estará disponible en línea.

---

## 📦 Requisitos

Crea un archivo `requirements.txt` con estas dependencias:

```
streamlit
pandas
numpy
openpyxl
```

---

## 📤 Salida del Reporte

El reporte se genera en pantalla en formato tabla y puede descargarse como archivo Excel con los indicadores por período. Los valores:
- Se muestran con **1 decimal**
- Las cifras monetarias están formateadas con **comas**
- Los valores relativos como el **ROE, ROA y Margen Neto** están expresados en **porcentaje**

---

## 🧾 Licencia

Este proyecto está licenciado bajo la licencia MIT.

---

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Abre un issue o haz un pull request con sugerencias o mejoras.