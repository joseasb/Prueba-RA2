# Prueba-RA2
Examen lenguajes marcas RA2

## **Ejercicio 1**
### *1A*
no se ve centrado porque no tiene un *flex-direction* en el .site-header. Poniendo *flex-direction: column* saldra centrado en el medio
---
### 1B

Usando Flexbox: en .site-header: usa *flex-direction: column

CSS grid con el display: grid

---
### 1C 
Para hacer dos filas dento del mismo header usamos **grid-template-rows: 1;**, creando asi una fila arriba, que es el h1, y otra abajo, que es la barra de navegacion


Para poder mostrar tanto en h1 con el nav, usamos en **.site.header** justify-items: center. Para el **nav** mas de lo mismo, usamos el justify-items: center.

Por ultimo, para poder separarlo 30 px, dentro de **.site.header** usamos **gap:30px** 

---
### 1D
Para la cabecera he usado un **background-color**, el color AQUA. Para que el contenido del header no se que quede "pegado" al borde. Para la separacion viual he usado un **border-radius:20px** para ponerle un borde a la cabecera de color "aqua" y un **box-shadow: 0 25px 20px rgba(0,0,0,0.1);** para ponerle una minima sombra debajo de la cabecera 
```
.site-header {
  display: grid;
  grid-template-rows: 1; 
  justify-items: center;         
  gap: 30px; 
  background-color: aqua; 
  box-shadow: 0 25px 20px rgba(0,0,0,0.1);
  padding:20px; 
  border-radius: 20px;
}
```

## **Ejercicio 2**
### 2A

He modificado el html, poniendo: 
```
**<button id="btn-menu" aria-label="Abrir menú">☰</button>** 
```
---
### 2B
Para maquetar ese diseño he introducido en el header **align-items: center;** y tambien un **justify-content: space-between;** haciendo que el primero centre el boton, el h1 y el nav de forma horizontal y el segundo los separa y y les deja espacio entre ellos
```
align-items: center;
justify-content: space-between;
```
## **Ejercicio 3**

### 3A
He creado nuevas miniaturas a partir de las imagenes ya seleccionadas y las miniaturas son de 200 px como piden y cuando haces clic en la miniatura se abre en otra pestaña 


<img width="285" height="392" alt="Captura de pantalla 2025-12-10 214014" src="https://github.com/user-attachments/assets/6fe57381-bb03-419e-ba15-c7f788803af4" />

---
### 3B

El efecto hover ya lo tenia incluido en el CSS cuando lo entregué, igualmente adjunto codigo y la demostracion 
```
.tarjeta:hover {
    box-shadow: 0 0 20px rgba(255, 0, 100, 0.4);
    transform: scale(1.1);


```
}<img width="1875" height="978" alt="Captura de pantalla 2025-12-10 214816" src="https://github.com/user-attachments/assets/c515f47c-5632-4ce3-bf09-e28c6b159d32" />

Como se ve en la imagen del artista "Steve Aoki", tiene un zoom y efecto de box-shadow cuando pasas el raton por encima

---
### 3C

Adjunto los cambios realizados en el html y el CSS y la imagen (lo hice ya en el apartado anterior pero bueno lo pongo aqui tambien porque aqui es donde lo pide :)

HTML CAMBIADO

```
 <section id="galeria" class="section">

            <h2>GALERIA DE ARTISTAS</h2>

            <div class="grid">
                <!-- TARJETA SIMPLE -->
                <div class="tarjeta">
                    <a href="ima/imAxwell.jpeg" target="_blank">
                    <img src="ima/imMINIATURAAxwell.jpg" alt="Axwell">
                    </a>
                    <p>Axwell es un DJ y productor sueco mundialmente reconocido, famoso por su participación en el trío Swedish House Mafia. Su estilo combina house progresivo, melodías emotivas y drops muy energéticos. Es considerado uno de los pilares del EDM moderno.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaTimmyTrumpets.jpeg" target="_blank">
                    <img src="ima/imaMINIATURATimmyTrumpets.jpg" alt="Axwell">
                    </a>
                    <h3>Timmy Trumpet</h3>
                    <p>Timmy Trumpet es un DJ y productor australiano conocido por mezclar EDM con trompeta en directo, creando un estilo único lleno de energía. Su música combina hardstyle, big room y sonidos latinos, con éxitos como Freaks o Narco.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaSteveAoki.jpeg" target="_blank">
                    <img src="ima/imaMINIATURASteveAoki.jpg" alt="Axwell">
                    </a>
                    <h3>Steve Aoki</h3>
                    <p>Steve Aoki es un DJ, productor y empresario estadounidense, uno de los artistas más explosivos del EDM. Famoso por sus shows intensos —incluyendo su clásico “cake face”— y sus colaboraciones con artistas de todo el mundo. Su estilo mezcla electro house, dubstep y música experimental.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaMartinGarrix.jpeg" target="_blank">
                    <img src="ima/imaMINIATURAMartinGarrix.jpg" alt="Axwell">
                    </a>

                    <h3>Martin Garrix</h3>
                    <p>Martin Garrix es un DJ y productor neerlandés que saltó a la fama mundial con solo 17 años gracias a su éxito Animals. Hoy es uno de los artistas más influyentes del EDM, conocido por su sonido progresivo, melodías épicas y actuaciones en los festivales más grandes del mundo.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaDavidGueta.jpeg" target="_blank">
                    <img src="ima/imaMINIATURADavidGueta.jpg" alt="Axwell">
                    </a>
                    <h3>David Guetta</h3>
                    <p>David Guetta es uno de los DJs y productores más influyentes de todos los tiempos. Considerado un pionero en llevar la música electrónica al mainstream, ha creado hits globales junto a artistas como Sia, Rihanna o Nicki Minaj. Su estilo va del house al pop electrónico.</p>
                </div>

                <div class="tarjeta">
                   <a href="ima/imaAvicii.jpeg" target="_blank">
                    <img src="ima/imaMINIATURAAvicii.jpg" alt="Axwell">
                    </a>

                    <h3>Avicii</h3>
                    <p>Avicii fue un DJ y productor sueco que revolucionó la música electrónica con su sonido melódico y emocional. Con himnos como Levels o Wake Me Up, fusionó el EDM con folk, pop y música acústica, dejando un legado imborrable en la industria. Es recordado como uno de los artistas más importantes de su generación.</p>
                </div>
            </div>
        </section>
```

CSS EFECTO HOVER YA HECHO
```
.tarjeta:hover {
    box-shadow: 0 0 20px rgba(255, 0, 100, 0.4);
    transform: scale(1.1);
}
```
<img width="1875" height="978" alt="Captura de pantalla 2025-12-10 214816" src="https://github.com/user-attachments/assets/f20949e7-0766-4cfc-b7af-3f2be3d5adfd" />


## **Ejercicio 4**

### 4.1. Introduccion

El tema de mi web consiste en el gran musical de musica electronica de Europa que se celebra cada año en Boom, Belgica, aunque tambien hay versiones fuera de Belgica. En mi pagina he incluido una serie de secciones. He incluido una portada con una foto de uno de los escenarios del festival y encima de la misma foto el titulo "Tomorroland" y una pequeña frase. Luego un pequeño inicio explicativo de "que es Tomorrowland", tambien de galeria de imagenes donde pongo a varios artistas que han actuado en el festival. Los tipos de entradas que hay junto a sus respectivos precios, junto a una seccion donde puedes "elegir" la entrada que quieres y por ultimo una seccion de contacto con informacion ficticia. Mi idea de diseño era hacer ver al usuario una pagina donde pueda saber un poco sobre el festival y sus artistas basandome, en cuanto a su diseño, en la pagina oficial de Tomorrowland


### 4.2. Evidencias de HTML5

En la seccion header lo que hago es poner la barra superior de la web, que incluye varias secciones dentro de la misma




<img width="451" height="224" alt="Captura de pantalla 2025-12-11 080509" src="https://github.com/user-attachments/assets/110f6bcf-1c15-40cf-9e60-b25b80cf4fae" />



<img width="1893" height="463" alt="Captura de pantalla 2025-12-11 080608" src="https://github.com/user-attachments/assets/c8ed5122-6e73-4f10-baf1-4cbbee064b95" />

El main basicamente incluyo todo el contenido de la pagina, desde la seccion **hero** hasta la seccion **contacto** en donde la modifico en el CSS

La seccion "**section**" lo que hay en poner de cada seccion de la seccion o aparatado de la pagina. Por ejemplo: en la imagen anterior he puesto la barra de nav con sus apartados, unos de ellos, por ejemplo es "inicio" pues su html es el siguiente


<img width="670" height="466" alt="Captura de pantalla 2025-12-11 081328" src="https://github.com/user-attachments/assets/4d90bfec-1140-420f-a473-21a940d0bac8" />

EL footer basicamente es la seccion final cuando llega un usuario indicando algun tipo de informacion, por ejemplo (que es muy tipico) los derechos de Copyright de la pagina o politicas de privacidad. En mi caso he puesto la fecha junto al curso e instituto

```
<footer class="footer">
         <p><a href="#hero">&copy; 2025 — 1º DAM, IES Saladillo</a></p>
    </footer>
```
---
El menu superior de la web es el "**header**", puesto anteriormente donde incluyo todas las secciones de la web 
```
 <header class="site-header">
        <nav class="top-menu">
            <a href="#hero">Inicio</a>
            <a href="#galeria">Galería</a>
            <a href="#tabla">Tipos de Entradas</a>
            <a href="#entrada">Entrada</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>
```

---
EL menu lateral lo hago de un "nav" donde pongo el mismo contenido del menu superior y sus secciones

<img width="320" height="125" alt="Captura de pantalla 2025-12-11 082136" src="https://github.com/user-attachments/assets/0929dc6b-09d3-421b-a17c-32672f404dcf" />


<img width="386" height="794" alt="Captura de pantalla 2025-12-11 082441" src="https://github.com/user-attachments/assets/f6bdb699-1d37-4d3a-8c40-16c2201e7c50" />

---
En la seccion "**hero**" ya lo hago dentro del main y es basicamente una foto en grande del festival, junto al titulo en grande que es *Tomorrowland* y una pequeña frase 


<img width="443" height="66" alt="Captura de pantalla 2025-12-11 082400" src="https://github.com/user-attachments/assets/87de2989-9e17-4237-9a1f-82bd014accdb" />



<img width="1881" height="716" alt="Captura de pantalla 2025-12-11 082519" src="https://github.com/user-attachments/assets/dadbbff2-2049-48db-9f77-abdca73fdf8c" />

(La tipografia y su diseño ya van dentro del CSS)

---
La tabla lo que hago es incluir los precios del festival junto a los dias que corresponde cada entrada, en la que creo un ```<div class="tabla-contenedor">``` para hacer el diseño de la tabla en su conjunto, y un ``` <table class="tabla">``` para modificar el contenido que hay dentro de la tabla. Sus tipos, precios, dias...
```
 <section class="section">
            <h2>PRECIOS PARA TU AVENTURA</h2>
                <div class="tabla-contenedor">
                    <table class="tabla">
                        <tr>
                            <th>Tipo</th>
                            <th>Precio</th>
                            <th>Duración</th>
                        </tr>
                        <tr>
                            <td>Day Pass</td>
                            <td>125€</td>
                            <td>1 día</td>
                        </tr>
                        <tr>
                            <td>Full Madness</td>
                            <td>295€</td>
                            <td>3 días</td>
                        </tr>
                        <tr>
                            <td>Comfort Pass</td>
                            <td>510€</td>
                            <td>3 días</td>
                        </tr>
                    </table>
                </div>
        </section>
```



<img width="1857" height="579" alt="Captura de pantalla 2025-12-11 083152" src="https://github.com/user-attachments/assets/0a9f3e4c-d04f-4c1b-b64f-5b3c65b267d3" />

---
El formulario es la seccion donde (ficticiamente) solicitas la entradas que tu quieres, en la que creo un  ``` <div class="caja-entrada">``` para modificar la "caja" , y que dentro van su contenido, y creo  ```  <form class="form"> ``` parar modificar lo que hay dentro de esa caja, poniendo un **label** para posteriormente poner un input que lo que hace es poner una "cajetilla" para poner lo que pide, por ejemplo, si el "label" es el nombre, abajo ponemos ``` <input type="text" required>``` en la que el "**text**" hace que ponga tu nombre, bueno, o lo que sea. Tambien he puesto un label, pero esta vez con opciones para escoger tu entrada, en la que abro "*select*" y dentro de ella pongo "*option*" que son opciones 
```
   <section id="entrada" class="section">
            <h2>¿QUE ENTRADA TE REPRESENTA? </h2>

            <div class="caja-entrada">
                <p> Ya sabes cómo puedes disfrutar Tomorrowland. Ahora decide cómo quieres vivir la experiencia.</p>

                <form class="form">
                    <label>Nombre:</label>
                    <input type="text" required>

                    <label>Email:</label>                       <---- pongo datos que me piden
                    <input type="email" required>

                    <label>Tipo de entrada:</label>
                    <select>
                        <option>Day Pass</option>
                        <option>Full Madness</option>           <---- pongo opciones
                        <option>Comfort Pass</option>
                    </select>

                    <button type="submit">Enviar</button>
                </form>
            </div>
        </section>

```

<img width="1236" height="822" alt="Captura de pantalla 2025-12-11 084644" src="https://github.com/user-attachments/assets/756a3835-5ec9-495a-a59d-f4ea2823d633" />
---
En la galeria de imagenes lo que incluyo en una serie de artistas que han participado en el festival en la que por cada artista abro el div ---> ```<div class="tarjeta">``` (todo dentro del mismo section) y pongo una imagen, el nombre del artista y una breve introduccion de quien es el artista para poner en contexto
```
  <section id="galeria" class="section">

            <h2>GALERIA DE ARTISTAS</h2>

            <div class="grid">
                <!-- TARJETA SIMPLE -->
                <div class="tarjeta">
                    <a href="ima/imAxwell.jpeg" target="_blank">
                    <img src="ima/imMINIATURAAxwell.jpg" alt="Axwell">
                    </a>
                    <p>Axwell es un DJ y productor sueco mundialmente reconocido, famoso por su participación en el trío Swedish House Mafia. Su estilo combina house progresivo, melodías emotivas y drops muy energéticos. Es considerado uno de los pilares del EDM moderno.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaTimmyTrumpets.jpeg" target="_blank">
                    <img src="ima/imaMINIATURATimmyTrumpets.jpg" alt="Axwell">
                    </a>
                    <h3>Timmy Trumpet</h3>
                    <p>Timmy Trumpet es un DJ y productor australiano conocido por mezclar EDM con trompeta en directo, creando un estilo único lleno de energía. Su música combina hardstyle, big room y sonidos latinos, con éxitos como Freaks o Narco.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaSteveAoki.jpeg" target="_blank">
                    <img src="ima/imaMINIATURASteveAoki.jpg" alt="Axwell">
                    </a>
                    <h3>Steve Aoki</h3>
                    <p>Steve Aoki es un DJ, productor y empresario estadounidense, uno de los artistas más explosivos del EDM. Famoso por sus shows intensos —incluyendo su clásico “cake face”— y sus colaboraciones con artistas de todo el mundo. Su estilo mezcla electro house, dubstep y música experimental.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaMartinGarrix.jpeg" target="_blank">
                    <img src="ima/imaMINIATURAMartinGarrix.jpg" alt="Axwell">
                    </a>

                    <h3>Martin Garrix</h3>
                    <p>Martin Garrix es un DJ y productor neerlandés que saltó a la fama mundial con solo 17 años gracias a su éxito Animals. Hoy es uno de los artistas más influyentes del EDM, conocido por su sonido progresivo, melodías épicas y actuaciones en los festivales más grandes del mundo.</p>
                </div>

                <div class="tarjeta">
                    <a href="ima/imaDavidGueta.jpeg" target="_blank">
                    <img src="ima/imaMINIATURADavidGueta.jpg" alt="Axwell">
                    </a>
                    <h3>David Guetta</h3>
                    <p>David Guetta es uno de los DJs y productores más influyentes de todos los tiempos. Considerado un pionero en llevar la música electrónica al mainstream, ha creado hits globales junto a artistas como Sia, Rihanna o Nicki Minaj. Su estilo va del house al pop electrónico.</p>
                </div>

                <div class="tarjeta">
                   <a href="ima/imaAvicii.jpeg" target="_blank">
                    <img src="ima/imaMINIATURAAvicii.jpg" alt="Axwell">
                    </a>

                    <h3>Avicii</h3>
                    <p>Avicii fue un DJ y productor sueco que revolucionó la música electrónica con su sonido melódico y emocional. Con himnos como Levels o Wake Me Up, fusionó el EDM con folk, pop y música acústica, dejando un legado imborrable en la industria. Es recordado como uno de los artistas más importantes de su generación.</p>
                </div>
            </div>
        </section>
```

<img width="1835" height="861" alt="Captura de pantalla 2025-12-11 084938" src="https://github.com/user-attachments/assets/aedd1977-18d7-4ca1-b62e-e922bf658c20" />

---

Los enlaces internos e externos---> Los internos lo que hago es abrir una nueva carperta y descargar los enlaces dentro de esa carpeta 


<img width="221" height="69" alt="Captura de pantalla 2025-12-11 085647" src="https://github.com/user-attachments/assets/c700ebc4-5006-4e64-b738-252ce854c640" />


Para los externos, directamente copio los enlaces de una web exterior y pongo de "**head**" ``` <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">```

## 4.3. Evidencias de CSS

Los selectores mas usados han sido "*class*" e "*id*" dentro de cada seccion con el suyo propio para modifcarlo en el CSS. Por ejemplo tengo
```

<div class="ticket">
                <h3>Day Pass</h3>
                <p class="ticket-descripcion"> Acceso válido para un solo día del festival. Ideal para quienes quieren
                    vivir
                    Tomorrowland de forma rápida pero intensa.</p>
                <ul>
                    <li>✔ Acceso a todos los escenarios durante ese día</li>
                    <li>✔ Shows principales del Mainstage</li>
                    <li>✔ Actividades tematizadas y áreas interactivas</li>
                    <li>✔ Acceso a zonas de comida, bebida y descanso</li>
                    <li>✔ Servicios básicos (baños, puntos de agua, etc.)</li>
                </ul>
            </div>
```
 Tengo el class "ticket" y el class "ticket-descripcion" dnetro del CSS. El class "ticket" modifica todo lo qu hay dentro, que generalmente lo que creo es una "cuadrado" donde pongo toda la informacion. E"ticket-descripcion" modifica solo el parrafo que empieza por "**Accede valido para un ...**"
```
.ticket {
    background: #222;
    padding: 20px;
    border-radius: 10px;
    border: 2px solid #c7a7ff;
    margin: 20px auto;
    max-width: 500px;
    text-align: left;
}
```
```
.ticket-descripcion {
    margin-bottom: 15px;
    opacity: 0.9;
}
```
<img width="954" height="492" alt="Captura de pantalla 2025-12-11 090910" src="https://github.com/user-attachments/assets/8f5f0e86-1b94-4996-b919-bd2685a27507" />
---
El pseudoclase que uso dentro de ese mismo "ticket" es un efecto hover en la que cuando paso en el raton por encima el fondo de ese "*ticket*" o "*cuadrado*" se vuelve se un color "**morado**"
```
.ticket:hover {
    background: #3a1a3a;
}
```


<img width="940" height="463" alt="Captura de pantalla 2025-12-11 091215" src="https://github.com/user-attachments/assets/f65ce905-9b57-4db8-9edc-8408b1503383" />

Se puede hacer una comparativa visual con la anterior imagen

---

Uso GRID para crear una cudricuala es la seccion de galeria, en la que el "**Display: grid**" activa la cuadricula de cada artista, el "**grid-template-columns: repeat(2, 1fr)**" lo que hace el poner cada artista, dos a cada lado y a continuacion otros dos aristas abajo y asi consecutivamente



<img width="897" height="872" alt="Captura de pantalla 2025-12-11 091925" src="https://github.com/user-attachments/assets/048d0d83-6f7d-4eeb-83be-fed4471dff5b" />



si por ejemplo; yo cambiara a "**repeat(3, 1fr)**", cada artista se pondria de tres en tres horizontamente


<img width="1143" height="886" alt="Captura de pantalla 2025-12-11 092119" src="https://github.com/user-attachments/assets/cac4aca8-149b-4c12-bf36-099ff757b5f0" />

y por ultimo un "**gap:20px**" para separar a cada artitas 20 pixeles

---

En esta misma galeria de artista hago uso del box shadow en la cuando paso en raton por encima, aparace una sombra "*rojiza*" alrededor del artista
```
.tarjeta:hover {
    box-shadow: 0 0 20px rgba(255, 0, 100, 0.4);
}
```
<img width="983" height="822" alt="Captura de pantalla 2025-12-10 214413" src="https://github.com/user-attachments/assets/c35329db-5cf9-49fb-a2a0-329107197730" /> 

--- 

Mis menus, tanto la barra de arriba como el menu deslizante son de un diseño simple. El menu de arriba esta fijado, es decir, es immovil, mediante "*position: fixed*", tiene una altura que ocupa de 70px en la que sus secciones esta centrada en centro del menu gracias al "*justify-content: center;*", cada seccion esta separada gracias al grid ---> "*gap:30px*" que lo separa 30px y cuando pasa el raton por encima de alguna de las secciones, la palabra de la tal seccion se pone de color rosa, o parecido gracias a efecto hover
```
.top-menu a:hover {
    color: #c7a7ff; /* color rosa Tomorrowland */
}
```
--- 
EL menu deslizante de boton tiene un estilo simple en la que le background es del mismo color que el menu de arriba y tambien tiene las misma secciones que el menu de arriba

## 4.4. Fuentes utilizadas


La fuente Local que he usado la siguiente **"CinzelDecorative", sans-serif** 



<img width="520" height="106" alt="Captura de pantalla 2025-12-11 093423" src="https://github.com/user-attachments/assets/8a3890eb-cbea-4bf0-a99b-8425bea4d9a4" />

--- 
Para la fuente Online he usado la siguiente 
```
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
```

----> **"Poppins", sans-serif**   Que uso en casi toda la tipografia de la web

---
Me han gustado mas estas tipografias porque considero que se adecua mas al estilo que tiene el Festival

## 4.5. Menú lateral: breve explicación

Lo que ocurre cuando pulso el boton es lo siguiente: Se abre un menu deslizante con cada de seccion de la pagina (Inicio, Galeria, Tipos de entradas...) en la que si pulsado la seccion que queremos visitar nos salta directamente a esa seccion, si pulsamos galeria, nos salta a la galeria de artistas. Si dejamos el raton por encima de la seccion nos saldra un saldra en efecto hover con un background

Ejemplo de lo ultimo
```
.side-menu a:hover {
    background: #333;
}
```

<img width="395" height="604" alt="Captura de pantalla 2025-12-11 094534" src="https://github.com/user-attachments/assets/18f90ad0-6b85-4f92-b70f-d9fc8e57388b" />


El icono del boton es justamente el logo oficial del festival, que cuando se abre, hace un giro de 90 grados y se "convierte" en una X, indicando que cuando se pulsa, se cierra el menu y vuelve a aparecer el logo

---
La clase que usa cuando pulsas el boton pasar a ser el "**.site-menu**"" 

```
.menu-btn {
    position: fixed;
    top: 15px;
    left: 15px;
    width: 45px; 
    height: 45px;
    display: flex; 
    align-items: center;
    justify-content: center;
    background: none;
    border: none;
    cursor: pointer;
    z-index: 4000; 
    transition: transform 0.3s ease; 
}



```
Ya tendria, para darle mas dinamismo, un activa  o un hover (background)
---

El menu con CSS se mueve con el side-menu 
```
<nav id="sideMenu" class="side-menu">
        <a href="#hero">Inicio</a>
        <a href="#galeria">Galería</a>
        <a href="#tabla">Tipos de Entradas</a>
        <a href="#entrada">Entrada</a>
        <a href="#contacto">Contacto</a>
    </nav>
```
```
.side-menu {
    position: fixed;
    top: 0;
    left: -230px; 
    width: 230px;
    height: 100vh;
    background: #111;
    padding-top: 60px; 
    transition: left 0.3s;
    z-index: 3000;
}

.side-menu.active {
    left: 0;
}

.side-menu a {
    display: block;
    padding: 15px 20px;
    color: white;
    text-decoration: none;
    border-bottom: 1px solid white; 
}

.side-menu a:hover {
    background: #333;
}
```

En "*.side-menu*", position: fixed lo que es cuando de abre el menu y tu te este moviendo por la pagina con el menu abierto, se quede inmovil. El left: -230px lo que hace es no se vea el menu hasta que le des al boton y el width hace que el menu ocupe 230 px a la derecha (lo contrario del left -230px). El "*transition: left 0.3s;*" hace que tenga una animacion deslizante cuando lo abres, es decir, que cuando lo abre se mueve el menu hasta ocupar 230 px y no se abra de una. 

 El: 
 ```
 .side-menu.active {
    left: 0;
}
```
hace que se muestre el menu desplazandolo a la derecha


## 4.6. Conclusión personal

Lo que he aprendido de este proyecto ha sido un poco mas entender algunos selectores que uso en el proyecto y como usarlo en el CSS. Me gustaria mejorar mas a la hora de entender mucho mas el CSS y como aplicar y entender mejor el Flexbox y el Grid. Lo que mas me ha costado ha sido hacer la seccion Hero (poner una foto y encima una imagen), con la dimesiones que queria y que se viera el titulo y el subtitulo centrado. La parte que mas me ha gustado de mi web ha sido la seccion de artistas, sobretodo el efecto hover de color rojizo que tiene al dejar el raton por encima
























