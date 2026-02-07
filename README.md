# Prueba Técnica: RPA PIX

## Descripción del Proyecto
* Este bot realiza la extracción diaria de productos, gestiona la base de datos local y sincroniza reportes con la nube, Finalmente se rellena el formulario y se adjunta el reporte generado
* Se utilizara **Pix RPA** y **C#** 

---

## Pasos para la Ejecución
* **Paso 1:** Clonar el repositorio en tu máquina local.
* **Paso 2:** Abrir el proyecto en **Pix RPA Studio**.
* **Paso 3:** Configurar las variables de entrada (argumentos) como las rutas de carpetas o credenciales. Esto sera desde el archivo guarado en /Data/Config.xlsx
* **Paso 4:** Ejecutar el flujo principal desde el Studio o mediante el ejecutable de Pix.

> [!IMPORTANTE]
> **Configuración API TOKEN:** El API TOKEN se genero statico en la  **[url](https://developer.microsoft.com/en-us/graph/graph-explorer)** Ejecutas cualquier GETa extraes el API Token y lo agregas al config.xlsx

---

## Requisitos o Dependencias
* **Software:** Es necesario tener instalado Pix RPA Studio versión 2.0 o superior.
* **Base de Datos:** El proyecto requiere un motor de **MYSQL** instalado o el driver correspondiente.
## Configuración de Base de Datos (MySQL)

El proyecto utiliza **MySQL** para el almacenamiento y procesamiento de datos. Sigue estos pasos para la configuración:

### Descargas Necesarias
Para que el bot pueda conectarse correctamente, necesitas instalar:

* **Servidor Local (XAMPP):** [Descargar XAMPP](https://www.apachefriends.org/es/download.html) (Asegúrate de iniciar el servicio MySQL).
* **Conector ODBC:** [Descargar MySQL Connector/ODBC](https://dev.mysql.com/downloads/connector/odbc/) (Requerido para la comunicación entre Pix y la BD).

> [!IMPORTANTE]
> **Configuración:** En el archivo `config.xlsx`, debes modificar la **Connection String** según las versiones de los servicios y el puerto que tengas configurado.

---
## Configuración del Navegador (WebDriver)
Por defecto, Pix y Selenium instalan la versión **1.45** de Chrome. Sin embargo, este proyecto fue desarrollado y probado con la versión **1.44**.

* **Solución:** En la raíz de este repositorio encontrarás el archivo `chromedriver.exe` de la versión 1.44.
* **Instalación:** Debes copiar dicho archivo y reemplazar el existente en la siguiente ruta de tu PC:
  `%AppData%\Local\PIX\WebDriver`

---

## Enlaces Importantes
Url del formulario utilizado para el desarrollo:

`https://form.jotform.com/260357630590053`



---
> [!TIP]
> **Nota:** Verificar el archivo Confi.xlsx para configurar los parametros segun sean requeridos para la correcta ejecucion del proyecto.