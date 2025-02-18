
```sh
#Construir la imagen Docker 
docker build -t jbrito1/jpbrito .

# Ejecutar el contenedor
docker run -d -p 80:80 jbrito1/jpbrito
