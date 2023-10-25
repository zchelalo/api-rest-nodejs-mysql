# api-rest-nodejs-mysql
API REST sencilla hecha con NodeJS y MySQL.  

## **Instalación:**  
Para probar la API debe tener instalado NodeJS (versión 18) y MySQL, una vez con eso listo clone el proyecto:  
```bash  
git clone https://github.com/zchelalo/api-rest-nodejs-mysql.git
```   
  
Despues de ello asegurese de estar dentro de la carpeta del proyecto y ejecute el siguiente comando:  
```bash  
npm i
```    
  
Una vez hecho esto puede probar la API ejecutando:  
```bash  
node src/index.js
```  
  
En caso de que quiera hacer un cambio y este se refleje automaticamente en el servidor deberá ejecutar el siguiente comando en lugar del anterior:  
```bash  
npm run dev  
```  
El comando anterior ejecutará el script asignado en el "package.json" el cual se llama "dev" el cual esta utilizando la librería de desarrollo nodemon.  
  
Con los requerimientos instalados deberá crear una base de datos en MySQL, la estructura que tendrá la base de datos ya esta creada en la carpeta "db" del proyecto, solo importe en su gestor de base de datos MySQL el archivo "database.sql" para crearla.  
  
Lo siguiente a hacer es el configurar las variantes de entorno en el archivo ".env.example", primeramente elegir el puerto de su preferencia, sus datos de configuración de MySQL, el nombre de la base de datos que acaba de crear y por ultimo modificar el archivo de las variables de entorno cambiandole el nombre, quitando el ".example" quedando solo así ".env". Quedando un archivo parecido al siguiente:  
```env  
PORT=3000

DB_HOST=localhost
DB_PORT=3306
DB_USER=root
DB_PASSWORD=password
DB_DATABASE=companydb
``` 