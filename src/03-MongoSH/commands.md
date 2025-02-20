
<!-- 
 CONECTARSE AL CONTENEDOR
 -->

docker-compose exec mongodb bash

<!-- 
CONECTADO AL MONGOSH
 -->

mongosh "url"

show dbs
show collections

<!-- 
CREAR Y USAR UNA BASE DE DATOS
-->
use("platzi_store")

<!-- 
INSERTAR DATOS
-->
db.productos.insertOne({
  name: "Producto 1",
  price: 1200
})

<!-- 
BUSCAR DATOS
-->
db.productos.find()  // Muestra todos los documentos en la colección productos

<!-- 
NOTA: Asegúrate de usar el nombre correcto de la colección:
- productos (plural)
- NO product
- NO producto
-->

