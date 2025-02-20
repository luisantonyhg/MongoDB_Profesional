<!-- 
LEVANTAR SERVICIO
 -->

docker-compose up -d mongodb
docker-compose ps  // Primera ejecución

<!-- 
RESULTADO DE LA PRIMERA EJECUCIÓN (con advertencia)
-->
time="2025-02-19T17:06:39-05:00" level=warning msg="C:\\Users\\32143695.BUHOPERU\\cursoMongoDB\\docker-compose.yml: the attribute `version` is obsolete, it will be ignored, please remove it to avoid potential confusion"
NAME                     IMAGE       COMMAND                  SERVICE   CREATED         STATUS         PORTS
cursomongodb-mongodb-1   mongo:5.0   "docker-entrypoint.s…"   mongodb   4 minutes ago   Up 4 minutes   0.0.0.0:27017->27017/tcp

<!-- 
RESULTADO DE LA SEGUNDA EJECUCIÓN (sin advertencia)
-->
docker-compose ps  // Segunda ejecución
NAME                     IMAGE       COMMAND                  SERVICE   CREATED         STATUS         PORTS
cursomongodb-mongodb-1   mongo:5.0   "docker-entrypoint.s…"   mongodb   4 minutes ago   Up 4 minutes   0.0.0.0:27017->27017/tcp
