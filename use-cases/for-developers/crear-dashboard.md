# Crear Dashboard

Para crear un dashboard primero se debe crear el registro en la aplicación en un grupo nuevo o en uno ya existente.

Este le dará la ruta de acceso al dashboard, además creara el permiso de acceso que posteriormente asignado a un "rol" permitirá al usuario con el permiso acceder al dashboard en su session en la aplicación.

<figure><img src="../../.gitbook/assets/registrar dashboard.gif" alt=""><figcaption><p>Crear Dashboard en Grupo</p></figcaption></figure>

Una vez creado el dashboard se podrá registrar consultas al mismo, estos servirán al momento de programar las graficas, podremos acceder a la data de las consultas con el nombre mediante el endpoint [http://{domain-name}/api/v1/queries/execute/\[name-endpoint\]](http://\{{host\}}/api/v1/queries/execute/\[name-endpoint]).

Para programar el dashboard creado se deberá crear un componente angular con la ruta generada en el modulo dashboard en el siguiente directorio en el proyecto:

`cocha-dashboard\cocha-dashboard-web\src\app\modules\dashboard\pages\`

Este directorio alberga todas las vistas de dashboards organizados de menara similar a los grupos en base a directorios.

Las tecnologías utilizadas para crear la vista de dashboards son las siguientes:

* tailwind (estilos)
* angular material (componentes, formularios)
* apache echart (graficas)

{% hint style="info" %}
Se puede utilizar otras librerias de graficos simplemente instalando la libreria deseada al proyecto.
{% endhint %}
