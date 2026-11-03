# Proyecto de analizis de regresion · Grupo Viva Cristo Rey

## Integrantes

- **Jose Garcia** — `josegdotcom`
- **[Nombre real]** — `[github-name]`
- **[Nombre real]** - `[github-name]`

## Entorno

El trabajo se realizará en el archivo `Proyecto.ipynb`, ya que este archivo hace posible usar el núcleo de R para el desarrollo. Como ya hemos trabajado con este formato antes, todos los integrantes del grupo están familiarizados con su ejecución y organización.

### Instalacion 

Para los palurdos incultos que no están familiarizados y no saben cómo hacer que Jupyter Notebook reconozca el kernel de R, aquí hay una solución.

1. **Instalen jupyter**
```bash
py -m pip install jupyter 
```
2. [**Instalen R.**](https://cran.r-project.org/bin/windows/base/)
3. Una vez instalado R o que ya estaba instalado; vayan a la carpeta `C:\Program Files\R\R-4.6.1\bin` y habran `R.exe`.
4. Dentro de la terminal, introduzcan la primera línea, respondan sí (con tilde) a todo y luego se les solicitará que seleccionen el *CRAN mirrow*, elijan el de Chile (que es administrado por la DCC, el final se aproxima). Una vez finalizado, ejecuten la segunda línea.
```bash
install.packages("IRkernel") 
```
```bash
IRkernel::installspec(user = TRUE)
```



## Descripcion

En este repositorio de github está el proyecto correspondiente al curso de análisis de regresión denominado *EYP230I*; este proyecto se enfocará en utilizar los conocimientos adquiridos durante el curso para desarrollar un modelo predictivo.
Los datos que se emplearán son de [Bike Sharing](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset), una colección de dos archivos en formato csv que contiene información semanal y diaria sobre el alquiler de bicicletas públicas en Nueva York, Estados Unidos, durante los años 2011 y 2012.

## Pregunta a responder

<div align="center">
    <h3>¿Cómo es afectado el número de bicicletas arrendadas con respecto a las condiciones climáticas, horario y fecha?</h3>
</div>

## Variable a predecir

Debido a que no se cual fue el feedback del profesor se **trabajara las variables 1 y 2** haciendo un doble analizis.

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
7. **holiday:** el tiempo es vacaciones o no.
8. **weekday:** día de la semana.
9. **workingday:** si el día no es ni fin de semana ni vacaciones es 1, de lo contrario es 0.
10. **weathersit:** Clara, pocas nubes, parcialmente nubladas, parcialmente nubladas.
11. **temp:** Temperatura normalizada en Celsius. Los valores se derivan a través de $\frac{t-t_{min}}{t_{max}-t_{min}}$, donde $t_{min}=-8$ y $t_{max}=+39$ (sólo en escala horaria).
12. **atemp:** Temperatura normalizada de sensación en Celsius. Los valores se derivan a través de $\frac{t-t_{min}}{t_{max}-t_{min}}$, donde $t_{min}=-16$ y $t_{max}=+50$ (sólo en escala horaria).
13. **hum:** Humedad normalizada. Los valores se dividen en 100 (max).
14. **windspeed:** Velocidad normalizada del viento. Los valores se dividen en 67 (max).
