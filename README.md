# Introduction

This notebook is part of [Applied Data Science with Python Specialization](https://www.coursera.org/specializations/data-science-python), especially the 2nd course [Applied Plotting, Charting & Data Representation in Python](https://www.coursera.org/learn/python-plotting?specialization=data-science-python).

"This assignment requires that you to find at least two datasets on the web which are related, and that you visualize these datasets to answer a question with the broad topic of weather phenomena (see below) for the region of Juiz de Fora, Minas Gerais, Brazil, or Brazil more broadly."

I choose to create a notebook that use [INMET](https://portal.inmet.gov.br/dadoshistoricos) (National Institute of Meteorology - Instituto Nacional de Meteorologia) to compare some measures between brazilian cities. This is the first part and it will be focus on collect the data. The second part was first built with Kaggle dataset [Brazil Weather, Automatic Stations (2000-2021)](https://www.kaggle.com/datasets/saraivaufc/automatic-weather-stations-brazil). However, considering that I want 2021 data updated, I create this first notebook to collect the data. I will make the files on Kaggle datasets.

## Data collection and summarization

The dataset presets the columns:

* ESTACAO / STATION
* DATA (YYYY-MM-DD) / DATE (YYYY-MM-DD)
* HORA (UTC) / TIME (UTC)
* PRECIPITACAO TOTAL HORARIO (mm) / TOTAL HOURLY RAIN (mm)
* PRESSAO ATMOSFERICA AO NIVEL DA ESTACAO, HORARIA (mB)  / ATMOSPHERIC PRESSURE AT STATION LEVEL, TIME (mB)
* PRESSAO ATMOSFERICA MAX.NA HORA ANT. (AUT) (mB) / MAX. ATMOSPHERIC PRESSURE IN THE PREVIOUS TIME. (AUT) (mB)
* PRESSAO ATMOSFERICA MIN. NA HORA ANT. (AUT) (mB) / ATMOSPHERIC PRESSURE MIN. IN THE EARLY TIME. (AUT) (mB)
* RADIACAO GLOBAL (W/m2) / GLOBAL RADIATION (W/m2)
* TEMPERATURA DO AR - BULBO SECO, HORARIA (C) / AIR TEMPERATURE - DRY BULB, TIME (C)
* TEMPERATURA DO PONTO DE ORVALHO (C) / DEW POINT TEMPERATURE (C)
* TEMPERATURA MAXIMA NA HORA ANT. (AUT) (C) / MAXIMUM TEMPERATURE IN THE PREVIOUS TIME. (AUT) (C)
* TEMPERATURA MINIMA NA HORA ANT. (AUT) (C) / MINIMUM TEMPERATURE IN THE PREVIOUS TIME. (AUT) (C)
* TEMPERATURA ORVALHO MAX. NA HORA ANT. (AUT) (C) / MAX DEW TEMPERATURE. IN THE EARLY TIME. (AUT) (C)
* TEMPERATURA ORVALHO MIN. NA HORA ANT. (AUT) (C) / DEW TEMPERATURE MIN. IN THE EARLY TIME. (AUT) (C)
* UMIDADE REL. MAX. NA HORA ANT. (AUT) (%) / REL HUMIDITY MAX. IN THE EARLY TIME. (AUT) (%)
* UMIDADE REL. MIN. NA HORA ANT. (AUT) (%) / REL HUMIDITY MIN IN THE EARLY TIME. (AUT) (%)
* UMIDADE RELATIVA DO AR, HORARIA (%) / RELATIVE AIR HUMIDITY, HOURS (%)
* VENTO, DIRECAO HORARIA (gr) / WIND, TIME DIRECTION (gr)
* VENTO, RAJADA MAXIMA (m/s) / WIND, MAXIMUM GUNS (m/s)
* VENTO, VELOCIDADE HORARIA (m/s) / WIND, HOUR SPEED (m/s)

The outputs will be:

* Weather year by year raw (weather_YYYY.zip)
* Weather year by year summarized (weather_sum_YYYY.zip)
* Weather summarized complete summarize (weather_sum.zip)
* Stations with them last record (stations.csv)

The dataset is available on Kaggle.
