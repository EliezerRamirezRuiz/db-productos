# METODOS API

URL_BASE = localhost:10000/api/

### PRODUCTO


<i> POST </i>   

- Producto/createProducto

> {
  "id": 1,
  "nombre": "Guitarra",
  "uri_imagen": "https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.istockphoto.com%2Fes%2Ffotos%2Fguitarra&psig=AOvVaw3dfui2GHHhLhGAGEyrqIT-&ust=1686632516899000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCOCJy536vP8CFQAAAAAdAAAAABAJ",
  "descripcion": "guitarras super chetada",
  "precio": 10000,
  "stock": [],
  "categoria": {
    "id": 1,
    "nombre": "Cuerda"
  }
}

</br>

<i> GET </i>

- [ Producto/getById/1 | Producto/getByNombre/Guitarra | Producto/getByPrecio/10000 | Producto/getByCategoria/1 ] 

> {
  "data": {
    "id": 1,
    "nombre": "Guitarra",
    "uri_imagen": "https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.istockphoto.com%2Fes%2Ffotos%2Fguitarra&psig=AOvVaw3dfui2GHHhLhGAGEyrqIT-&ust=1686632516899000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCOCJy536vP8CFQAAAAAdAAAAABAJ",
    "descripcion": "guitarras super chetada",
    "precio": 10000,
    "stock": [],
    "categoria": {
      "id": 1,
      "nombre": "Cuerdas"
    }
  }
}

</br>

### CATEGORIA
<i> POST </i>

- Categoria/createCategoria

> {
    "id":1,
    "nombre":"Cuerda"
}

</br>

<i> GET </i>

- [ Categoria/getById/1 | Categoria/getByNombre/Cuerda ]

> {
  "data": {
    "id": 1,
    "nombre": "Cuerdas"
  }
}