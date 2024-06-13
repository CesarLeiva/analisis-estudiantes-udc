# Análisis de Estudiantes UDC

Este repositorio contiene el análisis de datos obtenidos mediante scraping de LinkedIn, como parte del proyecto de grado "Sistema de Seguimiento a Personas mediante Algoritmos de Extracción de Contenido de Sitios Web".

## Tecnologías Utilizadas

- **Python**: Lenguaje principal para el procesamiento y análisis de datos.
- **Jupyter Notebook**: Para la visualización y análisis interactivo de datos.
- **Pandas**: Manipulación y análisis de datos.
- **Matplotlib**: Visualización de datos.
- **BeautifulSoup**: Extracción de datos de páginas web.
- **Requests**: Para realizar solicitudes HTTP.
- **Boto3**: Interacción con servicios de AWS, específicamente DynamoDB.
- **Python-dotenv**: Carga de variables de entorno desde un archivo `.env`.
- **JSON**: Formato de datos para almacenamiento y transferencia de datos estructurados.

## Descripción del Proyecto

El objetivo del proyecto es realizar un seguimiento de las trayectorias profesionales de los estudiantes de la Universidad de Cartagena (UDC) mediante el scraping de datos de LinkedIn y el acceso a datos almacenados en una base de datos DynamoDB. El análisis se centra en las experiencias laborales, las empresas en las que han trabajado y sus cargos.

## Estructura del Repositorio

- `analisis.ipynb`: Notebook con el análisis de datos.
- `Datos-experiencias-laborales.xlsx`: Archivo Excel con datos de experiencias laborales.
- `cargos.txt`: Lista de cargos obtenidos.
- `empresas.json`: Datos estructurados de empresas.
- `empresas_frecuencia_+2.txt`: Empresas con más de dos empleados UDC.
- `empresas_frecuencia_multiples.txt`: Empresas con múltiples empleados UDC.
- `empresas_frecuencia_uno.txt`: Empresas con un solo empleado UDC.
- `empresas_trabajando_actualmente.txt`: Empresas donde los estudiantes UDC trabajan actualmente.
- `udc-students-data.csv` y `udc-students-data.json`: Datos de estudiantes en formato CSV y JSON.

## Variables de Entorno

Para ejecutar este proyecto, se requieren las siguientes variables de entorno, que deben configurarse en un archivo `.env` en la raíz del proyecto:

- `AWS_ACCESS_KEY_ID`: Clave de acceso de AWS.
- `AWS_SECRET_ACCESS_KEY`: Clave secreta de AWS.

## Instalación y Ejecución

1. Clona el repositorio:
    ```bash
    git clone https://github.com/CesarLeiva/analisis-estudiantes-udc.git
    cd analisis-estudiantes-udc
    ```

2. Crea un entorno virtual e instala las dependencias:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3. Configura las variables de entorno en un archivo `.env`.

4. Recomendamos ejecutar el notebook desde Visual Studio Code. Para ello, instala la extensión "Jupyter":
    - Abre Visual Studio Code.
    - Ve a la sección de extensiones (icono de cuadrito en la barra lateral izquierda).
    - Busca "Jupyter" e instálala.

5. Abre el notebook en Visual Studio Code y ejecútalo:
    ```bash
    code analisis.ipynb
    ```

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue para discutir los cambios que deseas realizar.

## Licencia

Este proyecto está bajo la Licencia MIT.