# generacion_fake_news_gpt2
Generación de texto en formato noticias (titular + articulo) con gpt2 usando la libreria huggingface de python

## Como ejecutar los notebooks

Los notebooks están pensados para ejecutarlos en [Google Colab](https://colab.research.google.com/). El entorno de ejecución debe configurarse con GPU.

### Datos
Los datos se almacenan en Google Drive y se montan en la sección de Setup de los notebooks. Nosotros hemos trabajado con una carpeta en el inicio de nuestro Drive llamada spainai_webinar,
de ahí esta celda en la que cambiamos el directorio de trabajo a esa carpeta ```os.chdir('/content/drive/MyDrive/spainai_webinar')```. 
La estructura de carpetas debe ser:
```
 |-data  -> csv de entrada
 |-bows  -> txt con las bags of words de cada temática
 |-generated_headlines -> se escriben los txt con los headlines generados por el gpt-2 con pplm
 |-PPLM  -> carpeta que se crea al clonar al repo del PPLM (aquí se debe dejar el script run_pplm_mod.py
```
### Datasets

* Titulares y artículos: https://www.kaggle.com/snapcrack/all-the-news?select=articles1.csv

* Titulares de noticias deportivas: https://www.kaggle.com/rmisra/news-category-dataset

* Titulares de noticias financieras: https://www.kaggle.com/notlucasp/financial-news-headlines?select=guardian_headlines.csv

 
