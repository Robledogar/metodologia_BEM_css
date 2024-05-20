# Metodología BEM en CSS

## ¿Qué es BEM?
- BEM significa **B**lock **E**lement **M**odifier
- Es una metodología para nombrar y organizar tus clases CSS de forma clara y mantenible

## Componentes de BEM
### Block
- Representa una entidad independiente y autocontenida
- Puede ser un contenedor, un componente o un widget
- Utiliza `.bloque` como convención de nombre

### Element
- Representa una parte de un bloque y no tiene sentido por sí mismo
- Depende del bloque al que pertenece
- Utiliza `.bloque__elemento` como convención de nombre

### Modifier
- Representa un atributo, estado o variante de un bloque o elemento
- Cambia la apariencia o comportamiento del bloque o elemento
- Utiliza `.bloque--modificador` o `.bloque__elemento--modificador` como convención de nombre

## Ejemplo
```html
<div class="card">
  <h2 class="card__title card__title--large">Título de la tarjeta</h2>
  <p class="card__text">Texto de la tarjeta</p>
  <a href="#" class="card__link">Leer más</a>
</div>

```css
.card { /* Bloque */
  /* Estilos del bloque */
}

.card__title { /* Elemento */
  /* Estilos del elemento */
}

.card__title--large { /* Modificador de elemento */
  /* Estilos del modificador */
}

.card__text { /* Elemento */
  /* Estilos del elemento */
}

.card__link { /* Elemento */
  /* Estilos del elemento */
}

<!-- MAS EJEMPLOS -->

<!-- Bloque -->
<div class="header"></div>
<div class="button"></div>


<!-- Elemento-->
<div class="header">
    <h1 class="header__title"></h1>
    <nav class="header__nav"></nav>
</div>

<!-- Modificador -->
<button class="button button--primary"></button>
<button class="button button--secondary"></button>




