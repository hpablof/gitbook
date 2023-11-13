# 🖥 For Developers

La Aplicación esta formada for 2 principales componentes q utilizan las siguientes tecnologías:

Almacenamiento y extracción de datos:

* Data Warehouse - Postgres 14
* ETL - Pentaho 9.4

Aplicación visualización de datos smartcity:

* Backend API Rest - Laravel 10
* Frontend - Angular 15
* Cache - Redis 7
* Base Datos - Postgres 14

La aplicación web smartcity utiliza una propia base de datos para administrar usuarios, permisos y demás modelos que utiliza la aplicación, la información de consulta se encuentra separada de esta.

### Iniciar con Docker

Para iniciar el proyecto con docker y docker-compose el proyecto cuenta con archivos de configuración "docker-compose.yml" que inicia los siguiente procesos:

* api-rest
* frontend&#x20;
* cache
* database&#x20;

Para iniciar la aplicación primero se deberá hacer el build para posteriormente hacer correr los contenedores.

```bash
// build archivo defecto docker-compose.yml
docker-compose build 
// build archivo docker-compose-dev.yml
docker-compose -f docker-compose-dev.yml build
```

Dependiendo del ambiente (prod, dev) se deberá configurar los archivos de entorno en las siguientes rutas:

#### Produccion

/cocha-dashboard-api/.env.production

/cocha-dashboard-web/src/environments/environment.production.ts

#### Desarrollo

/cocha-dashboard-api/.env.development

/cocha-dashboard-web/src/environments/environment.development.ts



Una vez configurado los environments de  la aplicación se podra iniciar con el siguiente commando:

```bash
// run or restart default docker-compose.yml
docker-compose up -d 
// run or restart selected docker-compose file configuration path
docker-compose -f {compose file name} up
```

