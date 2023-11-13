---
description: >-
  La aplicación cuenta con distintos apartados de funcionalidad tanto de
  administración como usuario regular dependiendo el rol asignado.
---

# ✨ Nuestras Funcionalidades

<div>

<figure><img src="../../.gitbook/assets/Screenshot 2023-10-09 173153.png" alt=""><figcaption><p>Opciones para usuario administrador</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/Screenshot 2023-10-09 173248.png" alt=""><figcaption><p>Opciones para usuario registrado(sujeto a permisos asignado por administrador)</p></figcaption></figure>

</div>

El usuario **administrador** podra acceder a todas las funcionalidades tanto de administración como de vista de todos los dashboards.

El usuario **regular** solo podrá acceder al apartador de "Dashboards" y a las vistas q se le seran asignadas desde el lado de administración.

{% hint style="info" %}
**GitBook tip:** A succinct video overview is a great way to introduce folks to your product. Embed a Loom, Vimeo or YouTube video and you're good to go! We love this video from the fine folks at Loom as a perfect example of a succinct feature overview.
{% endhint %}

## Usuarios

{% hint style="info" %}
Apartado disponible solo para usuario con rol **Administrador.**
{% endhint %}

Este apartado permite la administración de usuarios que acceden a la aplicación.  Las funcionalidades disponibles son el listado a través de una tabla de datos, creación y edición de usuarios a través de un formulario y la eliminación con alerta de confirmación.

La tabla de listado de usuarios cuenta con paginación al pie de la pagina y con filtros por rol, estado y búsqueda de manera general, como se muestra en la imagen inferior.

<div align="left">

<figure><img src="../../.gitbook/assets/chrome-capture-2023-9-9.gif" alt=""><figcaption><p>Tabla de datos de usuarios con paginación y funcionalidad de filtros.  </p></figcaption></figure>

</div>

El registro y edición de usuarios se realiza a través de un formulario donde se llenan los datos de usuario, con las opciones de habilitado y asignación de rol en la aplicación. La opción de edición se encuentra en la columna de opcion en linea con el registro a editar

<figure><img src="../../.gitbook/assets/usuario-registro-actualizacion.gif" alt=""><figcaption><p>Registro y edición de usuarios</p></figcaption></figure>

La opción de eliminar usuario se encuentra en línea con el registro en la columna de opciones, antes de eliminar el registro mostrara una alerta de confirmación.

<figure><img src="../../.gitbook/assets/usuario-eliminar.gif" alt=""><figcaption></figcaption></figure>

## Roles y Permisos

{% hint style="info" %}
Apartado disponible solo para usuario con rol **Administrador.**
{% endhint %}

La administración de acceso a los diferentes dashboards se realiza a través de permisos que representan a un dashboard y estos van agrupados en roles q podrán ser asignados a los usuarios.

En la vista inicial se muestra todos los roles en la aplicación  con forma de tarjetas con el detalle de su nombre, cantidad de usuarios con el rol, las opciones de edición y eliminado y botón de registro de nuevos roles.&#x20;

<figure><img src="../../.gitbook/assets/smartcity.cochabamba.bo_users (1).png" alt=""><figcaption><p>Vista de roles en aplicación.</p></figcaption></figure>

El registro de un nuevo rol se realiza a través de un formulario donde se asigna el nombre y los dashboards a los cuales se otorgara acceso mediante el rol.

<figure><img src="../../.gitbook/assets/rol registrar.gif" alt=""><figcaption><p>Registrar nuevo Rol.</p></figcaption></figure>

Se puede acceder a la opción de edición de rol a través del botón bajo el nombre de cada rol, este desplegara un formulario con los datos del rol que se pueden editar.

<figure><img src="../../.gitbook/assets/rol editar.gif" alt=""><figcaption><p>Edición de datos de Rol.</p></figcaption></figure>

La opción de eliminado de rol se encuentra en la parte inferior izquierda de cada tarjeta de rol, este desplegara una alerta de confirmación para realizar la acción.

<figure><img src="../../.gitbook/assets/rol eliminar.gif" alt=""><figcaption><p>Eliminado de Rol.</p></figcaption></figure>

## Organizacion Dashboards

{% hint style="info" %}
Apartado disponible solo para usuario con rol **Administrador.**
{% endhint %}

Esta apartado administra la organización que se muestra en la sección de "Dashboards", los dashboards se organizan en grupos.

La vista inicial muestra una tabla con detalle de dashboards asociados al grupo, con una columna de opciones por registro con las funcionalidades de registro, edición y eliminado de grupo y dashboard, además de una función extra de endpoints por registro de dashboard que se vera mas adelante.

<figure><img src="../../.gitbook/assets/od-list.gif" alt=""><figcaption><p>Lista de grupos y dashboards.</p></figcaption></figure>

El registro de grupos se encuentra a lado del titulo principal, el registro de dashboards se realiza en la columna de opciones de cada fila de registro de grupo, ambos despliegan un formulario con los datos necesarios para el tipo de registro.

<figure><img src="../../.gitbook/assets/od-register.gif" alt=""><figcaption><p>Registro de Grupo y Dashboard</p></figcaption></figure>

La edición de información de grupo y dashboards se encuentra en la columna de opciones, este despliega un formulario donde se podrá actualizar la información deseada.

<figure><img src="../../.gitbook/assets/od editar.gif" alt=""><figcaption><p>Edición de grupo y dashboard.</p></figcaption></figure>

La función de eliminado de grupos y dashboards se encuentra en la columna de opciones del respectivo registro, este despliega una alerta de confirmación antes de realizar la acción.&#x20;

<figure><img src="../../.gitbook/assets/od-delete.gif" alt=""><figcaption><p>Eliminar Grupo o Dashboard.</p></figcaption></figure>

### Endpoints

Los endpoints son registros asociados al "dashboard" que manejan las consultas de datos necesarias para los gráficos e indicadores en las vistas. Estos tienes su propio apartado de administración con las funcionalidades de creación, edición y eliminado.

<figure><img src="../../.gitbook/assets/dashboards endpoints.gif" alt=""><figcaption><p>Panel de endpoints, consultas de datos q utiliza cada dashboard.</p></figcaption></figure>

{% hint style="info" %}
Solo se pueden registrar consultas de tipo sql "SELECT"
{% endhint %}

El panel muestra un formulario q permite registrar nuevas consultas de datos, además de un listado con una columna de opciones al final con  las acciones de editar y eliminar.&#x20;

## Embeddeds

{% hint style="info" %}
Apartado disponible solo para usuario con rol **Administrador.**
{% endhint %}

Registros de paginas diseñadas especialmente para ser embebidas en sitios externos.&#x20;

La vista inicial consta de un listado con una columna de opciones donde se puede agregar consultas al registro como en la sección [#endpoints](./#endpoints "mention"), editar información y eliminar.

<figure><img src="../../.gitbook/assets/smartcity.cochabamba.bo_organization-dashboards.png" alt=""><figcaption><p>Listado de embeddeds</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/embeddeds registrar, editar.gif" alt=""><figcaption><p>Registrar, editar embeddeds.</p></figcaption></figure>

## End Points

{% hint style="info" %}
Apartado disponible solo para usuario con rol **Administrador.**
{% endhint %}

Este apartado muestra una lista general de todos los registros de consulta creados tanto para paginas dashboard como paginas embebidas.

<figure><img src="../../.gitbook/assets/smartcity.cochabamba.bo_organization-dashboards (1).png" alt=""><figcaption><p>Vista general de endpoint creados para las diferentes paginas.</p></figcaption></figure>

## Home

La pagina "Home" es la pagina inicial al ingresar a la aplicación, dependiendo el rol del usuario se puede visualizar o todos los dashboard de datos creados o los asignados segun el administrador.

<figure><img src="../../.gitbook/assets/smartcity.cochabamba.bo_organization-dashboards (2).png" alt=""><figcaption><p>Vista home con vista general de dashboards creados.</p></figcaption></figure>

Las tarjetas de dashboards redirigen a la vista de dashboard deseada que de igual manera se puede acceder en el menu de navegacion sección de "dashboards".
