# ByteData



Esta clase fue añadida por un mod con la ID  `crafttweaker`. Necesitas tener este mod instalado si quieres usar esta caracteristica.

## Importar la clase
Puede ser requerido que importes el paquete si encuentras algun problema (como crear un Array).
```zenscript
crafttweaker.api.data.ByteData
```

## Interfaces implementadas
ByteData implementa las siguientes interfaces. Esto significa que cualquier método disponible también puede ser usado en esta clase.
- [data.IData](/vanilla/api/data/IData)
- [datos de crafttweaker.api.infumberData](/vanilla/api/data/INumberData)

## Constructores
```zenscript
new crafttweaker.api.data.ByteData(internal as byte);
```
| Parámetro | Tipo | Descripción                   |
| --------- | ---- | ----------------------------- |
| interno   | byte | No se proporcionó descripción |



## Métodos
### asList

Obtiene una lista<IData> la representación de esta IData, devuelve nulo en cualquier cosa menos [crafttweaker.api.data.ListData](/vanilla/api/data/ListData).

 Devuelve: `null si este IData no es una lista.`

Tipo de retorno: Lista&lt;[crafttweaker.api.data.IData](/vanilla/api/data/IData)&gt;

```zenscript
4.asList();
```

### asMap

Obtiene una representación del mapa<String, IData> de esta IData, devuelve nulo en cualquier cosa menos [crafttweaker.api.data.MapData](/vanilla/api/data/MapData).

 Devuelve: `null si este IData no es un mapa.`

Tipo de retorno: [crafttweaker.api.data.IData](/vanilla/api/data/IData)[String]

```zenscript
4.asMap();
```

### asString

Obtiene la representación de cadena de este IData

 Devuelve: `String que representa este IData (valor y tipo).`

Tipo de retorno: Cadena

```zenscript
4.asString();
```

### contiene

Comprueba si este IData contiene otra IData, utilizada principalmente en subclases de [crafttweaker. pi.data.ICollectionData](/vanilla/api/data/ICollectionData), es lo mismo que una comprobación igual en otros tipos IData

 Devuelve: `verdadero si el IData dado está contenido en este IData`

Tipo de retorno: booleano

```zenscript
4.contains(data as crafttweaker.api.data.IData);
4.contains("Mostrar");
```

| Parámetro | Tipo                                  | Descripción                              |
| --------- | ------------------------------------- | ---------------------------------------- |
| datos     | [data.IData](/vanilla/api/data/IData) | datos para comprobar si están contenidos |


### copiar

Hace una copia de este IData.

 IData es inmutable por defecto, use esto para crear una copia adecuada del objeto.

 Devuelve: `una copia de este IData.`

Tipo de retorno: [crafttweaker.api.data.IData](/vanilla/api/data/IData)

```zenscript
4.copy();
```

### getId

Obtiene el ID de la etiqueta NBT interna.

 Utilizado para determinar qué tipo de NBT se almacena (en una lista por ejemplo)

 Devuelve: `ID de la etiqueta NBT que representan estos datos.`

Tipo de retorno: byte

```zenscript
4.getId();
```

### getString

Obtiene la representación de cadena de la etiqueta INBT interna

 Devuelve: `Cadena que representa el INBT interno de este IData.`

Tipo de retorno: Cadena

```zenscript
4.getString();
```

