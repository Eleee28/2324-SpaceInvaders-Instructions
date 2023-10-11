# Preguntas Frecuentes

## Práctica 1


### Al resetear el juego, ¿el comportamiento aleatorio tiene que ser igual que al principio?

Sí, es necesario reutilizar la semilla (seed), es decir, hay que volver a crear el objeto Random con la misma semilla (`this.random = new Random(this.seed)`).

### La salida por consola muestra caracteres extraños, ¿qué ocurre?

Lo más probable es que la codificación que esté usando Eclipse no sea UTF-8. Para cambiarla:
- Selecciona el proyecto y pulsa el botón derecho seleccionando la opción *Properties*. 
- Elige el menú *Resource* y  comprueba que el valor de *Text File Encoding* es *UTF-8*. 
- En caso contrario, selecciona dicha opción.


### Tengo un método en `UCMLaser` que recibe un `RegularAlien` como parámetro para que el láser ataque al alien. ¿Tengo que añadir otro método para `DestroyerAlien`?

Sí, este es uno de los problemas que se mencionan en el enunciado: en nuestra solución deberemos copiar y pegar mucho código. El láser ataca (de la misma forma) a aliens, destroyer aliens, bombas y ovnis, de modo que necesitaremos
sobrecargar ese método y acabar teniendo cuatro versiones suyas: una que reciba como parámetro un `RegularAlien`, otro que reciba un `DestroyerAlien`, otr que recibea una `Bomb` y una última que reciba un `Ufo`. Las implementaciones de esos
métodos posiblemente sean idénticas entre sí (salvo por el tipo del objeto atacado).