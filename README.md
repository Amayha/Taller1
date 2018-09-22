Descripción de componentes UML taller 1 Ecosistemas  

 

Uml servidor en eclipse 

Main 

main(String[]):void : Con este método se ejecuta la aplicación 

Settings():void : Se usa para definir el tamaño del lienzo 

Setup():void: Aquí se definen todas las cosas que se ejecutan al iniciar el código 

Draw():void: Este método recibe todo la parte grafica visible en la pantalla 

Logica 

Logica(PApplet) : Construcctor de la logica 

pintar():void: Este método se utiliza para dibujar  

crearDulce():void: Este método es el que genera Object  de tipo Dulce , los cuales serán recogidos en el transcurso del juego 

choqueD():void: Este método es el que valida cuando un dulce es recogido por alguno de los personajes 

crearEnemigo():void: Este método es el que genera Object  de tipo Enemigo, los cuales serán recogidos en el transcurso del juego 

choqueE():void: Este método es el que valida cuando un enemigo choca con alguno de los personajes 

MoverFondo(): void: Este método se encarga de mover el mapa  

 

Objetos 

Objetos(PApplet, int, int) : void: Construcctor de los objetos 

mover (int,int):void: Este metodo se utiliza para realizar el cambio en la posición del personaje, enemigo o recogible 

// getters and setters 

getPosicionX():float: Se obtiene la posición horizontal del objeto 

getPosicionY():float: Se obtiene la posición vertical del objeto 

setPosicionX(float):void: Se cambia la posición horizontal del objeto 

setPosicionY(float):void: Se obtiene la posición horizontal del objeto 

getVida() : void: Se obtiene el número de vidas que tiene el objeto en cuestión 

setVida(int) : void: Se cambia el número de vidas que tiene le objeto en cuestión 

getVivo() : void: Se detecta si el objeto ha perdido todas sus vidas o sigue activo 

setVivo(boolean) : void: Se determina si el objeto deja de estar activo o no 

 

Servidor 

run():void: Es el hilo por el cual se establece la conexion con los clientes 

enviar () : void Envia los datos obtenidos por los botones al servidor 

Receptor 

Receptor(Socket ) : void: Construcctor del receptor 

run():void: Es el hilo por el cual se reciben los mensajes por parte de los clientes 

 

Princesa 

Princesa(PApplet, int, int) : void: Constructor del jugador1 

pintar():void: En este método se componen las imágenes que del jugador 

mover():void: En este método se general el cambio de posición 

 

Marceline 

Marceline(PApplet, int, int) : void: Constructor del jugador2 

pintar():void: En este método se componen las imágenes que del jugador 

mover():void: En este metodo se general el cambio de posicion 

 

Enemigo 

Enemigo(PApplet, int, int) : void: Construcctor del enemigo1 

pintar():void: En este método se componen las imágenes que del enemigo 

mover():void: En este método se genera el cambio de posición 

 

Dulce1 

Corazon(PApplet, int, int) : void: Construcctor del corazon 

pintar():void: En este metodo se crean las formas y/o imagenes que componen los corazones 

mover():void: En este metodo se general el cambio de posicion 

Dulce2 

Diamante(PApplet, int, int) : void: Construcctor del diamante 

pintar():void: En este metodo se crean las formas y/o imagenes que componen los diamantes 

mover():void: En este metodo se general el cambio de posicion 

Dulce3 

Estrella(PApplet, int, int) : void: Construcctor de la estrella 

pintar():void: En este metodo se crean las formas y/o imagenes que componen las estrellas 

mover():void: En este metodo se general el cambio de posicion 

 

 

Uml cliente en android studio 

Main 

onCreate (Bundle): void: Con este metodo se ejecuta la aplicacion 

Botones () : void Con este metodo se detectan las acciones de los botones 

Cliente 

Cliente(PApplet, int, int) : void: Construcctor del cliente 

run ( ): Recibe los datos enviados por parte del servidor 

enviar () : void Envia los datos obtenidos por los botones al servidor 

Receptor 

Receptor(Socket ) : void: Construcctor del receptor 

run ( ): Recibe los datos enviados por parte del servidor 

enviar () : void Envia los datos obtenidos por los botones al servidor 
