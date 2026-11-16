# Proyecto de análisis de regresión · Grupo Viva Cristo Rey

## Integrantes

- **Jose Garcia** — `josegdotcom`
- **Camila Rojas** — `Camila-Rojas-05`
- **Benjamín Ulloa** — `ReToxiE`

## Entorno

El trabajo se realizará en el archivo `Proyecto.ipynb`, ya que este archivo hace posible usar el núcleo de R para el desarrollo. Como ya hemos trabajado con este formato antes, todos los integrantes del grupo están familiarizados con su ejecución y organización.

### Instalación 

Para quienes no se encuentran familiarizados con el entorno y no saben cómo hacer que Jupyter Notebook reconozca el kernel de R, aquí hay una solución.

1. **Instalen jupyter**
```bash
py -m pip install jupyter 
```
2. Si no tiene instalado R,[**Instale R.**](https://cran.r-project.org/bin/windows/base/) de lo contrario, ignore este paso.
3. Ya con R instalado, vaya a la carpeta `C:\Program Files\R\R-4.6.1\bin` y abran `R.exe`.
4. Dentro de la terminal, introduzca la primera línea, responda sí (con tilde) a todo y luego se le solicitará que seleccionen el *CRAN mirrow*, elija el de Chile (que es administrado por el DCC, el final se aproxima). Una vez finalizado, ejecute la segunda línea.
```bash
install.packages("IRkernel") 
```
```bash
IRkernel::installspec(user = TRUE)
```



## Descripción

En este repositorio de github esta el proyecto correspondiente al curso de análisis de regresión denominado *EYP230I* ; este proyecto se enfocará en utilizar los conocimientos adquiridos durante el curso para desarrollar un modelo predictivo.
Los datos que se emplearán son de [Bike Sharing](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset), una colección de dos archivos en formato csv que contiene información diaria y por hora sobre el alquiler de bicicletas públicas en Washington D.C. Estados Unidos, durante los años 2011 y 2012.

## Pregunta a responder

<div align="center">
    <h3>¿Cómo es afectado el número de bicicletas arrendadas con respecto a las condiciones climáticas, horario y fecha?</h3>
</div>

## Variable a predecir

Debido a que no se cual fue el feedback del profesor se **trabajara las variables 1 y 2** haciendo un doble análisis.

1. **casual:** La cantidad de personas no suscritas que arrendaron una bicicleta.
2. **registered:**  La cantidad de personas suscritas al servicio que arrendaron una bicicleta.
3. **cnt:** conteo de bicicletas de alquiler totales, incluyendo tanto casuales como registrados.


## Variables disponibles

1. **instant:** índice de registro.
2. **dteday:** Fecha.
3. **season:** 1: winter, 2: spring, 3: summer, 4: fall.
4. **yr:** año (0: 2011, 1: 2012).
5. **mnth:** mes (1 a 12).
6. **hr:** hora (0 a 23).
7. **holiday:** el tiempo es feriado o no.
8. **weekday:** día de la semana (0: Domingo, 1: Lunes, ... , 6: Sabado).
9. **workingday:** si el día no es ni fin de semana ni feriado es 1, de lo contrario es 0.
10. **weathersit:** Clara, pocas nubes, parcialmente nubladas, parcialmente nubladas.
11. **temp:** Temperatura normalizada en Celsius. Los valores se derivan a través de $\frac{t-t_{min}}{t_{max}-t_{min}}$, donde $t_{min}=-8$ y $t_{max}=+39$ (sólo en escala horaria).

12. **atemp:** Temperatura normalizada de sensación en Celsius. Los valores se derivan a través de $\frac{t-t_{min}}{t_{max}-t_{min}}$, donde $t_{min}=-16$ y $t_{max}=+50$ (sólo en escala horaria).

13. **hum:** Humedad normalizada. Los valores se dividen en 100 (max).
14. **windspeed:** Velocidad normalizada del viento. Los valores se dividen en 67 (max).
