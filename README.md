# Taller de Posicionamiento + Float en CSS

![Resultado](/images/result.png)

Autor: Eduardo Oviedo Blanco

Para usar este taller efectivamente, clone el código en su ambiente local.
```
git clone https://github.com/edWAR6/CSS-Positioning-Float-Workshop.git
```
Si desea subir el taller en su repositorio personal.
Cree un repositorio en su perfil, luego:
```
git remote set-url origin https://github.com/<tu usuario>/CSS-Positioning-Float-Workshop.git
```

> El nombre del repositorio puede cambiar. Siga las instrucciones y guarde sus cambios.

## Instrucciones

1. Asegúrese de que el elemento `div-1a` tenga solo un párrafo y que el `div-1b` tenga dos.

2. Para lograr tener columnas dentro de un contenedor sin un tamaño fijo, puede usar la propiedad `float`.
```
#div-1a {
  ...
  float: left;
  width: 50%;
}
```

> Note como el contenedor es extendido verticalmente, esto siempre y cuando la causa sea un elemento **no** flotante.

3. Ahora convierta dos de los *div* hijos en columnas flotantes.
```
#div-1a {
  ...
  float: left;
  width: 33%;
}
```
```
#div-1b {
  ...
  float: left;
  width: 33%;
}
```

> Note como ahora el problema regresa.
> Debido a que ahora el elemento que controla el alto del padre tiene poco contenido, los elementos flotantes sobresalen del padre.

4. Para solucionarlo, puede repararlo con la propiedad `clear`.
```
#div-1c {
  ...
  clear: both;
}
```

## Conclusión

Es recomendable usar estas técnicas para solucionar problemas pequeños, ya que hoy en día existen técnicas mejores y más modernas como flex-box y el grid system.
