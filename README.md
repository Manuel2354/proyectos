# Análisis ESG vs Rendimiento (2016–2025)

Este proyecto combina análisis cuantitativo y sostenibilidad para identificar las empresas con mayor rendimiento financiero y mejor calificación ESG, tanto en México como en Estados Unidos, durante el periodo 2016–2025.

##  Objetivo

Evaluar si existe una correlación entre alto desempeño financiero y buen puntaje ESG, con base en datos históricos de mercado y calificaciones sostenibles proporcionadas por S&P Global.

## Herramientas utilizadas

- Python (Pandas, NumPy, yfinance)
- Jupyter Notebook
- Excel (para importar las calificaciones ESG)
- Power BI (para visualización final)
- VS Code y/o GitHub

##  Metodología

1. Se descargaron precios históricos de acciones con `yfinance`, desde enero 2015 hasta junio 2025.
2. Se calcularon rendimientos acumulados por ticker, usando la fórmula:
   Rendimiento = (Precio final - Precio inicial) / Precio inicial
3. Se manejaron valores nulos y `inf` para evitar errores en la agregación.
4. Se integró el archivo Excel con calificaciones ESG.
5. Se filtraron las 5 empresas con:
- Mayor ESG Score
- Mayor rendimiento acumulado
- Separado por país (MEX / USA)
6. Se exportó el DataFrame final a Excel y se visualizó en Power BI.

##  Visualización

El resultado se presenta en un tablero creado en Power BI, que muestra:

- Top 5 empresas por país
- Comparativa entre ESG Score y Rendimiento
- Identificación de empresas líderes en sostenibilidad y desempeño

![ESG](https://github.com/user-attachments/assets/3185282a-34ec-4dbb-ba56-ea94a3af09de)


## Archivos

| Archivo                  | Descripción                                        |
|--------------------------|----------------------------------------------------|
| `ESG_criterios.ipynb`    | Código Python completo con limpieza, merge y cálculos |
| `ESG Score.xlsx`         | Calificaciones ESG por empresa (S&P Global Score) |
| `ESG.pbix`               | Reporte visual en Power BI                         |
| `ESG.xlsx`               | Output final con los datos combinados              |
| `ESG.jpg`                | Imagen del dashboard exportado                    |

## 📌 Notas

- Nota: El rendimiento acumulado fue calculado como la suma de los rendimientos diarios. Este enfoque permite extender el análisis hacia periodos específicos (por ejemplo, por año) o construir comparativas evolutivas en el tiempo.
- El código es escalable para incluir nuevos criterios o países en el futuro.

## Autor

**Manuel Gallegos Sánchez**  
Contador, analista de inversiones y entusiasta de las finanzas cuantitativas.  
[LinkedIn](https://www.linkedin.com/in/manuel-gallegos-s%C3%A1nchez)

----




