# XML del gestor de un sistema informático de jardinería
### Repositorio sobra la tarea de un almacén de pedidos

```
  <?xml version="1.0" encoding="iso-8859-15" standalone="yes" ?>

<!DOCTYPE elementos [
	<!ELEMENT elementos (plantas, flores, utensilios*)
		<!ELEMENT plantas (planta)+>
			<!ELEMENT planta (#PCDATA)>
				<!ATTLIST planta
				nombre CDATA #REQUIRED
				>
		<!ELEMENT flores (flor)+>
			<!ELEMENT flor (#PCDATA)>
				<!ATTLIST flor
				color CDATA #IMPLIED
				>
		<!ELEMENT utensilios (utensilio)*>
			<!ELEMENT utensilio (numero)>
				<!ELEMENT numero (#PCDATA)>
				
]>

<elementos>
	<plantas>
		<planta nombre="Pata de elefante"/>
		<planta nombre="Helecho"/>
		<planta nombre="Bonsai"/>
		<planta nombre="Medinilla"/>
	</plantas>
	<flores>
		<flor color ="amarillo">Girasol</flor>
		<flor color ="rosa">Rosa</flor>
	</flores>
	<utensilios>
		<utensilio>Pala</utensilio>
      <numero>1</numero>
		<utensilio>Pico</utensilio>
      <numero>1</numero>
		<utensilio>Cubo</utensilio>
      <numero>2</numero>
		<utensilio>Saco</utensilio>
      <numero>3</numero>
	</utensilios>
</elementos>
```

Este es mi código. Tal y como pedía el ejercicio, creé una etiqueta que contuviera las etiquetas "plantas", "flores" y "utensilios". A su vez, definí la estructura del código para añadir atributos y elementos obligatorios, u optativos, según fuera necesario. Al final, en el XML coloqué varios ejemplos para observar la estructura del código. 
