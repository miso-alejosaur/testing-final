# Entrega Final

## Instrucciones para ejecutar tests - Kraken

### Prerequisitos
* Tener instalado Node Version (14.17.0)

### Instalación - Ghost - Version 4.44.0
Para la creación de estos test, se usó la versión 4.44.0 de Ghost; para ejecutar esta versión, ubíquese mediante consola en el directorio donde tenga instalado Ghost, y ejecute los siguientes comandos:
```
ghost uninstall
ghost install 4.44.0 -local
```
Cuando la instalación finalice, se iniciará la ejecución de Ghost en `http://localhost:2368`, en caso que inicie en otro puerto o dirección, modifiquelo en el archivo `Kraken/properties.json`, en la propiedad HOST.
### Configuración del sitio
Ingrese a la url http://localhost:2368/ghost/ (si su instancia de Ghost se ejecutó en otro puerto, úselo); allí encontrará un formulario para crear un nuevo Sitio en ghost. En los campos "Site title" y "Full name" ingrese los datos que desee, en el campo "Email Address" ingrese `test@test.tt`, y en el campo "Password" ingrese `1234567890a.`. Estas son las credenciales configuradas en Kraken; en caso de configurar otra combinación de usuario y contraseña, será necesario que modifique estos datos en el archivo `Kraken/properties.json`.
![imagen](https://user-images.githubusercontent.com/98656893/167307021-8f72da03-575a-4cdc-89a5-50dcf7e8a2eb.png)

### Ejecución de las pruebas y ubicación de los screenshots
Una vez creado el sitio, ubíquese mediante consola en el directorio `/Kraken` (perteneciente a este repositorio), y allí ejecute el comando 
```
npm install
```
Una vez node instale todas las dependencias, ejecute el comando 
```
node_modules/kraken-node/bin/kraken-node run
```
Verá que comienza la ejecución de las pruebas en Kraken. Tras la finalización de la ejecución, verá dentro de la carpeta `screenshots`, los pantallazos tomados por Kraken para cada uno de los pasos, en cada uno de los escenarios.

# Otros entregables

- [Estrategia de Pruebas](https://github.com/miso-alejosaur/testing-final/blob/main/estrategia-pruebas-final.pdf)
- [Pruebas Manuales/Exploratorias](https://github.com/miso-alejosaur/testing-final/blob/main/inventario-pruebas-exploratorias.xlsx)
- [Issues reportados](https://github.com/miso-alejosaur/testing-final/issues)

# Miembros del equipo

- Alejandro Santamaría Pérez (a.santamaria11@uniandes.edu.co)
- Andrés Javier Oviedo Morales (a.oviedom@uniandes.edu.co)
- Steve Andersson Rojas Hernández (s.rojash@uniandes.edu.co)
- Washington Roberto Parra Vásquez (w.parrav@uniandes.edu.co)
