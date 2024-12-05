
# Batalla de Equipos Digimon

Una aplicación web interactiva desarrollada con Flask que permite a los usuarios seleccionar Digimon para formar dos equipos y enfrentarlos en una batalla simulada. ¿Qué equipo tendrá el mayor poder?

## Características

- **Selección de equipos:** Elige hasta 6 Digimon para cada equipo.
- **Cálculo de poder total:** Visualiza el poder total acumulado de cada equipo.
- **Batalla simulada:** Descubre cuál equipo es el más fuerte.
- **Interfaz interactiva:** Diseño atractivo y dinámico con confeti y animaciones.

## Requisitos previos

Asegúrate de tener lo siguiente instalado en tu sistema:

- **Python 3.7 o superior**
- **Docker** (opcional, para ejecutar la aplicación en un contenedor)

## Instalación local

1. **Activa el entorno virtual**:

   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Instala las dependencias(si no las tiene instaladas)**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Ejecuta la aplicación**:

   ```bash
   python app.py
   ```

5. **Accede a la aplicación**:

   Abre tu navegador y ve a `http://localhost:5000`.

## Despliegue con Docker

1. **Construye la imagen de Docker**:

   ```bash
   docker build -t digimon-team-battle .
   ```

2. **Ejecuta el contenedor**:

   ```bash
   docker run -p 5000:5000 digimon-team-battle
   ```

3. **Accede a la aplicación**:

   Ve a `http://localhost:5000` en tu navegador.

## Archivos principales

- **`app.py`:** Contiene la lógica principal de la aplicación.
- **`templates/index.html`:** Página principal con la interfaz para seleccionar equipos y realizar la batalla.
- **`static/css/style.css`:** Estilos personalizados para la aplicación.
- **`static/js/scripts.js`:** Lógica del cliente para manejar la selección de equipos y la simulación de la batalla.
- **`Dockerfile`:** Configuración para construir la imagen de Docker.
- **`requirements.txt`:** Lista de dependencias necesarias para ejecutar la aplicación.

## Cómo usar

1. Selecciona hasta 6 Digimon para cada equipo.
2. Presiona el botón **"Enfrentar Digimones"** para calcular el poder total y determinar el equipo ganador.
3. Limpia los equipos con los botones correspondientes si deseas realizar una nueva batalla.

## Créditos

- **Framework:** Flask
- **API utilizada:** [Digimon API](https://digimon-api.vercel.app/)

## Licencia

Este proyecto se encuentra bajo la licencia MIT. Siente la libertad de usarlo, modificarlo y compartirlo.
