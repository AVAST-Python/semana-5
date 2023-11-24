

# Pandas ultrarápido

---

# Cambio de punto de vista

- No estás manejando Excels: estás haciendo Data Analysis
- Excel sólo es tu soporte. Tú estás trabajando con los datos.
- Lo importante es el proceso de los datos.
- Aprende a analizar los datos y te dará igual el soporte


---

# Objetivo de hoy:

### abrir un excel y obtener las filas que cumplen una condición

---

# Enlaces:

- [Introducción a Pandas](https://aprendepython.es/pypi/datascience/pandas/)
- [Fichero de pruebas](/ejemplo1.xlsx)

---

# Previo: instalar las dependencias

```bash
pip install pandas
pip install xlwt openpyxl xlsxwriter xlrd
```
<!-- .element style="font-size: 1em" -->

- Debes trabajar con Python 3. Testealo con `python --version`
- Muy recomendable usar `venv`, pero eso para otro día
- [`pandas`](https://pandas.pydata.org/) es la librería principal para manejo de datos. Tiene "tol power".
- El resto son librerías para acceder a ficheros Excel

---

# Cómo abrir un Excel

```python
import pandas as pd

import os
import pathlib
current_dir = pathlib.Path(__file__).parent.resolve()

file = os.path.join(current_dir, '..', 'datos','ejemplo1.xlsx')

xls = pd.ExcelFile(file)
df = pd.read_excel(xls, 'Hoja1')
```
<!-- .element style="font-size: 1em" -->
- Esto siempre va a ser igual
- Lo que te va a devolver es un DataFrame
- En la siguiente diapositiva tienes más información

---

# Ejercicio:

- Revisa el siguiente enlace y ves leyendo hasta que puedas hacer el ejercicio:
  [https://aprendepython.es/pypi/datascience/pandas/](https://aprendepython.es/pypi/datascience/pandas/)

- Avísame en caso de atasco
- Te llevará un tiempo, al principio puede sonar marciano
- No te cortes en buscar por Internet o preguntar a ChatGPT, pero asegúrate de que entiendes lo que estás haciendo. Si no
  lo entiendes, intenta hacerlo a mano.




