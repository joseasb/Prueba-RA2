# Prueba-RA2
Examen lenguajes marcas RA2

## **Ejercicio 1**
### *1A*
no se ve centrado porque no tiene un *flex-direction* en el .site-header. Poniendo *flex-direction: column* saldra centrado en el medio

### 1B

Usando Flexbox: en .site-header: usa *flex-direction: column

CSS grid con el display: grid


### 1C 
Para hacer dos filas dento del mismo header usamos **grid-template-rows: 1;**, creando asi una fila arriba, que es el h1, y otra abajo, que es la barra de navegacion


Para poder mostrar tanto en h1 con el nav, usamos en **.site.header** justify-items: center. Para el **nav** mas de lo mismo, usamos el justify-items: center.

Por ultimo, para poder separarlo 30 px, dentro de **.site.header** usamos **gap:30px** 


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

### 3B

El efecto hover ya lo tenia incluido en el CSS cuando lo entregué, igualmente adjunto codigo y la demostracion 
```
.tarjeta:hover {
    box-shadow: 0 0 20px rgba(255, 0, 100, 0.4);
    transform: scale(1.1);


```
}<img width="1875" height="978" alt="Captura de pantalla 2025-12-10 214816" src="https://github.com/user-attachments/assets/c515f47c-5632-4ce3-bf09-e28c6b159d32" />

Como se ve en la imagen del artista "Steve Aoki", tiene un zoom y efecto de box-shadow cuando pasas el raton por encima

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





