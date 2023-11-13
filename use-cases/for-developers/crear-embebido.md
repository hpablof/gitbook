# Crear Embebido

La creación de un embebido consta de primeramente crear el registro en la aplicación en el apartado de embeddeds, a este registro se podra agregar consultas de datos que serán accesibles con el nombre registrado.

[#embeddeds](../../vision-general/nuestras-funcionalidades/#embeddeds "mention") <- como crear un registro embedded

<figure><img src="../../.gitbook/assets/registrar endpoints.gif" alt=""><figcaption><p>Agregar consultas de datos a registro de embebido.</p></figcaption></figure>

La parte visual debe ser programada en el proyecto web de la aplicación, en el modulo de **embedded,** directorio pages donde se debe generar un nuevo componente angular y la ruta.

`cocha-dashboard\cocha-dashboard-web\src\app\modules\embedded\pages`&#x20;

Los componentes, estilos, librerias para crear la parte visual son las siguientes.

* tailwindcss (estilos)
* angular material (componentes, formularios)
* apache echarts (gráficos)

{% hint style="info" %}
Desde el componente se podrá hacer peticiones de datos con los nombres de consulta creados para el registro embebido anteriormente, mandando peticiones al endpoint:

&#x20;[http://{domain-name}/api/v1/queries/execute/\[name-endpoint\]](http://\{{host\}}/api/v1/queries/execute/\[name-endpoint])


{% endhint %}

