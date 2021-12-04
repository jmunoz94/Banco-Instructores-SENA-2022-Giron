# Puntajes Banco de Instructores SENA 2022 (BANIN-2022)
Puntajes generales del Banco de Instructores SENA 2022 del Centro Industrial de Mantenimiento Integral (Girón, Santander).

## Prerrequisitos

Para la lectura de pdfs se utilizan los bindings de Python para Apache Tika. Para su ejecución, es necesario tener un servidor de Tika en ejecución. 

Hay múltiples formas de configurar uno, una de las más sencillas se describe dentro del notebook. Sin embargo, para poder ejecutar Tika se requiere tener Java instalado y configurado en el equipo.

## Instalación

Se recomienda crear un ambiente virtual. Puede hacerlo de la forma que le resulte más conveniente, una forma de hacerlo es:

```bash
python -m venv .sena
```

Con el comando anterior se crea un ambiente llamado `.sena`, usted puede asignarle el nombre que desee.

Active su ambiente virtual:

Windows:
```bash
.sena\Scripts\activate
```

Linux o Mac:
```bash
source .sena\bin\activate
```

Una vez tenga su ambiente virtual creado y activo, instale las dependencias:

```bash
pip install -r requirements.txt
```

## Uso

El código se encuentra en un notebook de Jupyter. Hay muchas formas de ejecutar notebooks, una de ellas es ejecutar el siguiente comando en el directorio raíz (la carpeta en donde esté este proyecto, al no tener subcarpetas, no debería haber lugar a confusión):

```bash
jupyter notebook
```

Se abrirá el navegador con un explorador de archivos. Ubique `banin_2022_parser.ipynb` y ábralo haciendo clic en él.

Siéntase libre de modificar el código. Algunas opciones pueden ser adaptarlo para calcular los puntajes de otro centro o determinar el 60% del puntaje que depende de las pruebas para todos los que aplicamos a la convocatoria del banco de instructores 2022.

## Resultados

Si solamente está interesado en el archivo de resultados para el Centro Industrial de Mantenimiento Integral, descargue el archivo `ResultadosSENA2022.xlsx`. 

En este archivo encuentra cuatro hojas con la siguiente información:
* `Generales`: Puntajes totales, organizados de mayor a menor, con desglose de la contribución de cada uno de los tres criterios (hoja de vida, prueba habilidades digitales y prueba socioemocional).
* `Hoja de Vida`: Puntajes de la hoja de vida, organizados de mayor a menor, con el puntaje real (escala de 0 a 100) y estandarizado (escala de 0 a 40).
* `Prueba Habilidades Digitales`: Puntajes de la prueba de habilidades digitales, organizados de mayor a menor, con el puntaje real (escala de 0 a 100) y estandarizado (escala de 0 a 20).
* `Prueba Socioemocional`: Puntajes de la prueba socioemocional, organizados de mayor a menor, con el puntaje real (escala de 0 a 100) y estandarizado (escala de 0 a 40).