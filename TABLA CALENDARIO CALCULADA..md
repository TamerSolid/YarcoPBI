TABLA CALENDARIO CALCULADA. 



Calendario = CALENDAR(DATE(YEAR(TODAY())-1,1,1),DATE(YEAR(TODAY())+2,1,1))



**COLUMNAS**

Mes = MONTH(Calendario\[Date])

Year = YEAR('Calendario'\[Date])

**Mes Nombre = FORMAT(Calendario\[Date], "MMMM")**

**Mes Corto = FORMAT(Calendario\[Date], "MMM")**

**Trimestre = "Q" \& FORMAT(Calendario\[Date], "Q")**

**Año-Mes = FORMAT(Calendario\[Date], "YYYY-MM")**

**Semana Número = WEEKNUM(Calendario\[Date], 2)  -- semana inicia en lunes**

**Día = DAY(Calendario\[Date])**

**Día de la Semana Número = WEEKDAY(Calendario\[Date], 2)  -- lunes = 1**

**Día de la Semana Nombre = FORMAT(Calendario\[Date], "dddd")**

**Es Fin de Semana = IF(WEEKDAY(Calendario\[Date], 2) > 5, TRUE(), FALSE())**

**Es Hoy = IF(Calendario\[Date] = TODAY(), TRUE(), FALSE())**

**Es Pasado = IF(Calendario\[Date] < TODAY(), TRUE(), FALSE())**

**Es Futuro = IF(Calendario\[Date] > TODAY(), TRUE(), FALSE())**

**Es Día Laboral = IF(WEEKDAY(Calendario\[Date], 2) < 6, TRUE(), FALSE())**

**Inicio de Mes = DATE(YEAR(Calendario\[Date]), MONTH(Calendario\[Date]), 1)**

**Fin de Mes = EOMONTH(Calendario\[Date], 0)**

**Inicio de Semana = Calendario\[Date] - WEEKDAY(Calendario\[Date], 2) + 1**

**Fin de Semana = Calendario\[Date] + (7 - WEEKDAY(Calendario\[Date], 2))**



