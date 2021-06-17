# SUBASTA-UTEC

**SUBASTAS UTEC es un sistema en tiempo real escrito en Flask. En el lado del BACKEND, se utiliza Flask para cambios en tiempo real en los objetos publicados. En el lado de FRONTEND, se utiliza MaterializeCSS para mostrar todo el diseño. 

Características:
- `Flask-WTF` para la creación y validación de formularios
- `Flask-SQLAlchemy` para acceso a la base de datos
- `Flask-Admin` para un panel de control sencillo sobre las acciones en la plataforma
- `Flask-SocketIO` para actualización de valores en tiempo real
- `TinyPNG` para la compresión de imágenes de perfiles y artículos
- Registro con ** reCaptcha ** para protegerse del spam y el abuso
- Hash de contraseñas con ** PBKDF2 ** para reducir las vulnerabilidades a los ataques de fuerza bruta

## Vista previa

Verifique en [http://aukcije-online.herokuapp.com] (http://aukcije-online.herokuapp.com). Debería cargarse en unos segundos si el dinamómetro no funciona.

Puede usar el nombre de usuario `dummy` y la contraseña` dummy123` para mirar alrededor y explorar (* crear un artículo, actualizar el perfil y ofertar por artículos *)

Página de destino:

! [Página de destino] (extras / landing-page.png "Página de destino")

Página de perfil:

! [Página de perfil] (extras / profile-page.png "Página de perfil")

Página del artículo:

! [Página del artículo] (extras / article-page.png "Página del artículo")


## Instalar y ejecutar localmente

1. Vaya a la ubicación deseada donde desea colocar el proyecto y clonar usando `git clone https://github.com/dinko-pehar/flask-realtime-auction.git && cd flask-realtime-Auction`
2. Crea un entorno virtual 
3. Con el entorno virtual activado, instale las dependencias usando pip como `pip install -r requirements.txt`
4. (* OPCIONAL *) Exporte `RECAPTCHA_PUBLIC_KEY` y` RECAPTCHA_PRIVATE_KEY` para usar * reCaptcha * en el formulario de registro. Puede generar claves en https://www.google.com/recaptcha/intro/v3.html
5. Con `flask run`, ejecutará y expondrá la aplicación en el puerto * 5000 *

---

Una alternativa a lo anterior es compilar y ejecutar la aplicación dentro del contenedor Docker como:

1. `docker build -t aukcije: latest .`
2. `docker run --rm -ti p 5000: 5000 aukcije`

## Contribuir y usar
Las solicitudes de extracción son bienvenidas. Bifurque, reescriba o use esta aplicación de la forma que desee.

## Licencia
[MIT] (https://choosealicense.com/licenses/mit/)
