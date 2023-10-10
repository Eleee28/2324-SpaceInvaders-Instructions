# Preguntas Frecuentes

## Práctica 1


### Al resetear el juego, ¿el comportamiento aleatorio tiene que ser igual que al principio?

Sí, es necesario reutilizar la semilla (seed), es decir, hay que volver a crear el objeto Random con la misma semilla (`this.random = new Random(this.seed)`).

### La salida por consola muestra caracteres extraños, ¿qué ocurre?

Lo más probable es que la codificación que esté usando Eclipse no sea UTF-8. Para cambiarla:
- Selecciona el proyecto y pulsa el botón derecho seleccionando la opción *Properties*. 
- Elige el menú *Resource* y  comprueba que el valor de *Text File Encoding* es *UTF-8*. 
- En caso contrario, selecciona dicha opción.