---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-01"

---

{:new_window: target="_blank"}  
{:shortdesc: .shortdesc}


# Adición de una nueva credencial de servicio
{: #service_credentials}

Puede generar un nuevo conjunto de credenciales de servicio para casos en los que quiera conectarse manualmente un consumidor externo a un servicio de Bluemix. Por ejemplo, si está intentando enlazar una app de AWS a un servicio Watson, necesitará generar una nueva credencial de servicio que se pueda utilizar para enlazar estos dos servicios.

Los servicios de Cloud Foundry pueden generar una clave de servicio, también conocida como credencial de servicio. Las credenciales de servicio son específicas del servicio y varían en función de cómo define cada servicio las credenciales que necesita generar. Una credencial de servicio puede contener un nombre de usuario, una contraseña, un nombre de host, un puerto y una URL. Sin embargo, el contenido de cada credencial de servicio es exclusivo para el servicio que la genera. Algunos servicios pueden generar datos adicionales que requieren que se pasen parámetros. Por ejemplo, un servicio puede necesitar que especifique un parámetro de idioma para establecer el idioma predeterminado devuelto en la clave de servicio que se genera. 

Siga estos pasos para añadir una nueva credencial de servicio:

1. En la página de detalles de servicio, seleccione el separador Credenciales de servicio, y pulse **Credencial nueva + **.
2. En el diálogo Añadir credencial nueva, proporcione un **Nombre**.
3. Opcionalmente, puede proporcionar parámetros adicionales como objeto JSON válido que contiene parámetros de configuración específicos del servicio, proporcionados en línea o en un archivo.

  **Nota**: La mayoría de los servicios no requieren parámetros adicionales, y para los servicios que sí los requieren, cada servicio define su propia lista exclusiva de parámetros. Para obtener una lista de parámetros de configuración soportados, consulte la documentación para ver la oferta de servicios concreta.
4. Pulse **Añadir** para generar la nueva credencial de servicio.
