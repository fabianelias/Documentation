## Flask
  
FLask es un framework ligero de aplicaciones web. Está diseñado para que el inicio sea rápido y fácil, con la capacidad de escalar hasta aplicaciones complejas. Comenzó como un simple envoltorio alrededor de Werkzeug y Jinja y se ha convertido en uno de los frameworks de aplicación web Python más populares.
Flask ofrece sugerencias, pero no impone ninguna dependencia ni diseño del proyecto. Depende del desarrollador elegir las herramientas y bibliotecas que quiere usar. Hay muchas extensiones proporcionadas por la comunidad que facilitan la incorporación de nueva funcionalidad.  
#### Instalación 
Para instalar y actualizar Flask ejecuta lo siguiente:
~~~
pip install -U Flask
~~~

A continuación un ejemplo simple utilizando Flask
~~~
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
    return 'Hello, World!'
~~~

Luego por terminal podemos ver el resultado: 
~~~
$ FLASK_APP=hello.py flask run
 * Serving Flask app "hello"
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
~~~