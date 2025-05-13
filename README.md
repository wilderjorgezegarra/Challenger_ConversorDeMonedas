<h1 align="center"> Challenger Conversor de Moneda </h1>

## Descripción de su proyecto:
    Aplicación en Java para convertir diferentes monedas utilizando el API ExchangeRate.


## Funcionalidades:
    Conversión
 de monedas en tiempo Real.
       - USD ↔ ARS
       - USD ↔ BRL
       - USD ↔ COP
       - OTRAS ↔ MONEDAS  

## a.- Utilizamos la herramienta Trello.
       Utilizamos la herramienta de colaboración/gestión Trello para seguir una secuencia ordenada en el desarrollo del aplicativo conversor de moneda challenger one java backend.

## b.- Utilizamos la WEB de Exchange Rate API.
       Para el proyecto hemos elegido la Exchange Rate API, con sus tasas de cambio en tiempo real, que nos proporciona información precisa y actualizada en conversión de moneda.
       - Para obtener la clave API nos hemos remitido a la página de ExchangeRate-API cuyo link es: https://www.exchangerate-api.com/
       - No registramos para obtener nuestra clave: https://v6.exchangerate-api.com/v6/0956f5f484a510157254d675

## c.- Utilizamos Postman la plataforma para la gestión de APIs.
       Herramienta para testear APIs de tipo Rest, también cuenta con una serie de métodos que nos permiten tomar acción ante nuestras peticiones que son:
       - GET: Obtener información
              Realizando la consulta al GET:  https://v6.exchangerate-api.com/v6/0956f5f484a510157254d675/pair/ 
       - POST: Agregar información
       - PUT: Reemplazar la información
       - PATCH: Actualizar alguna información
       - DELETE: Borrar información

       Resultado del link; muestra los tipos conversión de monedas:
        {
            "result": "success",
            "documentation": "https://www.exchangerate-api.com/docs",
            "terms_of_use": "https://www.exchangerate-api.com/terms",
            "time_last_update_unix": 1746576001,
            "time_last_update_utc": "Wed, 07 May 2025 00:00:01 +0000",
            "time_next_update_unix": 1746662401,
            "time_next_update_utc": "Thu, 08 May 2025 00:00:01 +0000",
            "base_code": "USD",
            "conversion_rates": {
                "USD": 1,
                "AED": 3.6725,
                "AFN": 71.1199,
                "ALL": 86.8437,
                "AMD": 389.5887,
                        ..
                        ..
            }
        }

## d.- Utilizamos el lenguaje de programación Java.
    Estamos utilizando Java:
        - Versión versión "17.0.14" 2025-01-21 LTS
        - Java(TM) SE Runtime Environment (build 17.0.14+8-LTS-191)
        - Java HotSpot(TM) 64-Bit Server VM (build 17.0.14+8-LTS-191, mixed mode, sharing)

    Creamos las siguientes clases:
        - Creando Clase: Principal
        - Creando Clase-Record: Monedas
        - Creando Clase: ConsultaMoneda
        - Creando Clase: ConvertirMoneda
        - Creando Librería Gson: Gson (gson-2.10.1.jar) para convertir objetos Java a JSON(Formato de texto ligero para almacenar y transportar datos) de ExchangeRate-API.

    Creamos el siguiente menú para el conversor de monedas.
        "Bienvenido/a al Conversor de Moneda.\n\n"+
        "Ingrese la conversión que deseas realizar.\n\n"+
        "1.- Dólar => Peso Argentino\n"+
        "2.- Peso Argentino => Dólar\n"+
        "3.- Dólar => Real Brasileño\n"+
        "4.- Real Brasileño => Dólar\n"+
        "5.- Dólar => Peso Colombiano\n"+
        "6.- Peso Colombiano => Dólar\n"+
        "7.- Convertir otra moneda => Dólar\n"+
        "8.- Salir");

    Ejemplo01: Ejecución de nuestra aplicación de la conversión de 1 moneda elegida en el según menú de opciones.
        Elija una Opción :
        1
        La conversion para hoy de: [USD] equivale a 1203.83 [ARS]
        Ingrese el valor que desea convertir USD
        1
        El valor 1.0 [USD] corresponde al valor final de 1203.83 [ARS]
        ************************************

    Ejemplo02: Ejecución de nuestra aplicación de la conversión de 1 moneda, en la opción 7 ingresando la moneda que deseo que deseo convertirlo.
        Elija una Opción :
        7
        Ingrese el código de la moneda Base
        eur
        Ingrese la moneda objetivo: 
        usd
        La conversion para hoy de: [EUR] equivale a 1.1341 [USD]
        Ingrese el valor que desea convertir EUR
        1
        El valor 1.0 [EUR] corresponde al valor final de 1.1341 [USD]

## e.- Utilizamos GitHub.
    Utilizamos el GitHub para alojar y compartir nuestro código.  https://github.com/wilderjorgezegarra/Challenger_ConversorDeMonedas.git


## Estructura del Proyecto.
    Carpeta Principal: Challenger_ConversorDeMonedas
    - .git.- Es una carpeta que indica que está siendo gestionado por Git, un sistema de control de versiones distribuido. Esta carpeta oculta contiene toda la información necesaria para rastrear los cambios en los archivos y versiones del proyecto.
    - .idea.- Es una carpeta oculta que contiene la configuración del proyecto, no del código fuente. Tiene almacenada la información específica del proyecto como configuraciones de ejecución, depuración.
    - out.- Carpeta donde se guardan los archivos .class de los resultados de la compilación.
    - src.- Carpeta principal donde se ubican los archivos fuente de código Java (.java).
    - .gitignore.- Archivo de texto que se coloca en la raíz de un repositorio Git y que indica a Git qué archivos o carpetas deben ser ignorados y no rastreados para el control de versiones.
    - Challenger_ConversorDeMonedas.iml.- El un archivo que guarda la configuración y las características del módulo del proyecto. Es un archivo XML que contiene metadatos y configuraciones clave para que el IDE entienda y gestione la estructura y las dependencias del módulo.


## Entorno de Desarrollo(IDE).
    Utilizamos el IntelliJ IDEA 2024.3.5(Community Edition), para desarrollar el proyecto en Java pues nos ofrece un entorno de desarrollo inteligente y eficiente para aumentar la productividad y la calidad del código.


## Licencia
    Este proyecto es de código abierto y está disponible bajo la licencia MIT. Siéntete libre de usarlo y adaptarlo a tus necesidades.


## Persona que Desarrolla el Proyecto.
    Alumno de Alura Latam G8: Wilder, JORGE ZEGARRA.


## Asesoría.
    Aplicación Discord y preguntas en el FORO de Alura Latam ONE Student Oracle, que nos orientan muy bien. 
