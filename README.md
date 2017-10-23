# Space Shooter
Este proyecto hecho con Unity siguiendo el tutorial de https://unity3d.com/es/learn/tutorials/projects/space-shooter-tutorial/

## Explicacion del juego
El juego se basa en una nave que tiene que destruir asteroides que nos van  apareciendo en el mapa y tenemos que destruirlos para evitar la colision. para ello cree un gameobject player que seria nuestra nave.

## Nave
En la nave estaria formada por un objeto que seria un gameobject situado en la parte frontal de la nave que seria el punto de spawn de los disparos, desde este punto se crean los disparos que serian otro game object que se crea cada vez que clickamos la pantalla y se mueven hacia adelante segun la velocidad que le indiquemos con una cdencia determinada por una variable editable, y el gameobject de la naev en si.
El script de la nave es PlayerController en el manejo lo qe seria el movimiento usando el Accelerometro y el evento del click para generar Objetos que le apsariamos por parametro en este caso los Disparos

## Entorno
El juego en si esta formado por el fondo, la nave y los asteroides. Estos elementos estan dentro de un cubo el cual destruye todo lo que colisione con el, con esto solucinamos la creacion de objetos infinitos en el espacio que nos consumirian espacio como los disparos y los asteroides que salgan fuera del alcance.

## Asteroides
Los asteroides son un objeto que tiene asociado unos scripts scripts(DestroyByContact, RandomRotator), en el primero gestiono lo que seria la destruccion por contacto, dependiendo si esta en contacto con un shot o el jugador hara una animacion de explosion u otra.
En el rotator hago un generacion de rotacion aleatoria para el objeto asteroide para si dar una sensacion que los asteroides son diferente ya que cada uno rotara de forma diferente segun se vayan creando.
