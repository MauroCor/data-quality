# Data Quality

Este repositorio contiene la configuración y utilidades necesarias para validar la calidad de tus datos utilizando Great Expectations, facilitando la integración de pruebas de calidad en tus flujos de trabajo de datos.

## ¿Qué es Great Expectations?
Great Expectations es una herramienta open source para validar, documentar y perfilar la calidad de los datos. Permite definir expectativas sobre los datos, automatizar pruebas y generar reportes visuales para asegurar la confiabilidad de los datos en procesos de análisis y machine learning.

---

## Requisitos
- Python 3.7+
- [Great Expectations](https://greatexpectations.io/) (`pip install great_expectations`)

## Instalación
1. Clona este repositorio.
2. Instala las dependencias necesarias:
   ```bash
   pip install great_expectations
   ```
3. (Opcional) Configura tu entorno de datos en `great_expectations/`.

## Ejecutar un checkpoint
Ejecuta las expectativas definidas en un checkpoint:
```bash
great_expectations checkpoint run <nombre_del_checkpoint>
```
Ejemplo:
```bash
great_expectations checkpoint run test
```

## Ver el reporte
Después de ejecutar un checkpoint, abre el reporte HTML generado:
```bash
xdg-open great_expectations/uncommitted/data_docs/local_site/index.html
```

---
Para más información, consulta la [documentación oficial](https://docs.greatexpectations.io/).

