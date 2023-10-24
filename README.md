# SemanaTec12-23-Oct-23
# Nombre: Erick Schiller Echavarria
# Matricula: A01740804
# Carrera: ITC
# Semestre: 5to
## Practica de GitHub
# Integrante de Equipo: Emilio Rizo de la Mora A01721612

**Bold Semana Tec12**
*Italic*

1. Hot-cakes 🥞
2. Tacos Barbacoa 🌮
3. Chilaquiles 🍲
4. Galletas Oreo 🍪
5. Huevo Estrellado 🍳

---
- Piano
- Guitarra
- Bajo
- Motolina
- Flauta
---

```
"""Paint, for drawing shapes.

Exercises

1. Add a color.
2. Complete circle.
3. Complete rectangle.
4. Complete triangle.
5. Add width parameter.
"""

from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
```

| Nombre | Actividad |
| -------- | -----------|
| Yeseli | Dibujar un auto |
| Carolina | Dibujar un pastel |
| Hubert | Dibujar tigre |

- [x] Yeseli dibujar auto
- [x] Carolina dibujar pastel
- [x] Hubert dibujar tigre


# SemanaTecArteProgra
Para crear un encabezado, agrega uno o 6 símbolos # antes del encabezado del texto.

# Encabezado grande 
## Encabezado mediano
### Encabezado pequeño

Puedes indicar énfasis con texto en negritas, itálicas o tachadas en los campos de comentario

Estilo
- Negrita ** ** **Este texto está en negritas**
- Cursiva * * __ *Este texto está en cursiva*
- Tachado ~~ ~~ ~~Este texto está equivocado~~
- Cursiva en negrita y anidada ** ** y __ **Este texto es _extremadamente_ importante**
- Todo en negrita y cursiva *** *** ***Todo este texto es importante***
# Usar emojis inicia escribiendo : + letra escoges el emoji que quieres
🍎.
👏🏿.
🥇.
🥈.
🥉.
|
# Cita de Texto
> ITESM

# Enlace [GitHub Pages](https://pages.github.com/)

#Imagen
![GitHub Pages](https://tex.mx/sites/default/files/repositorio/Home/tex-de-monterrey-newsroom.jpg)

# SemanaTecOct 2021

```geojson
{
    "type": "Polygon",
    "coordinates":[
        [
            [-85,35],
            [-100.2155, 25.6748],
            [-100.309, 25.6714],
            [-101.35628, 20.67675],
            [-85, 30]
        ]
    ]
}
```
# Listas
Puedes realizar una lista desordenada al anteceder una o más líneas de texto con - o *.

- Panda Rojo
- Ron da error
- Los Picapiedra

1. Panda Rojo
2. Ron da error
3. Los Picapiedra

# Listas Anidadas
- Primer Concierto
    - Primer pijamada
        - Panda

#Lista de Tareas
- [X] #739
- [ ] 👩🏻
- [x] Emilio Dibujar un rectangulo
 
