# Camión de transporte

Una empresa de transporte quiere administrar mejor las cargas que lleva un camión.

Para eso requiere un sistema que le permita planificar qué cosas debe llevar el camión y si sobrepasa su capacidad. Por otro lado, las cosas que transporta tienen un nivel de peligrosidad. Este nivel es usado para impedir que cosas que superen cierto nivel de peligrosidad circulen en rutas.

## Parte 1
### El camión

- Se pide que se le pueda cargar y descargar cosas (de 1 a vez) y también cual es el peso total del camión, incluyendo su tara que es de 1000 kg. 
- También se necesita conocer si los pesos de todas las cosas cargadas en el camión son números pares. 
- Debemos poder consultar si hay alguna cosa que pesa un determinado valor.
- Para un mejor control del tipo de peligro que puede representar la carga, se debe poder obtener la primer cosa cargada que tenga un determinado nivel de peligrosidad 
- Obtener todas las cosas que superan un determinado nivel de peligrosidad. 
- Para facilitar los controles, también nos piden que se pueda consultar la lista de cosas que superan el nivel de peligrosidad de una cosa dada.
- Conocer si el camión está excedido del peso máximo permitido,que es de 2500 kg. 
- Saber si el camión puede circular en ruta. Eso depende de que no exceda el peso máximo permitido y ninguno de los objetos cargados supere un nivel máximo de peligrosidad que depende del viaje, por eso para este caso el valor del nivel se pasará como argumento.


### Las cosas
De las cosas que puede transportar el camión nos interesa el peso y la peligrosidad. Por ahora conocemos las siguientes:

* Knight Rider: pesa 500 kilos y su nivel de peligrosidad es 10.
* Bumblebee: pesa 800 kilos y su nivel de peligrosidad es 15 si está transformado en auto o 30 si está como robot.
* Paquete de ladrillos: cada ladrillo pesa 2 kilos, la cantidad de ladrillos que tiene puede variar. La peligrosidad es 2.
* Arena a granel: el peso es variable, la peligrosidad es 1.
* Batería antiaérea : el peso es 300 kilos si está con los misiles o 200 en otro caso. En cuanto a la peligrosidad es 100 si está con los misiles y 0 en otro caso.
* Contenedor portuario: un contenedor puede tener otras cosas adentro. El peso es 100 + la suma de todas las cosas que estén adentro. Es tan peligroso como el objeto más peligroso que contiene. Si está vacío, su peligrosidad es 0.
* Residuos radioactivos: el peso es variable y su peligrosidad es 200.
* Embalaje de seguridad: es una cobertura que envuelve a cualquier otra cosa. El peso es el peso de la cosa que tenga adentro. El nivel de peligrosidad es la mitad del nivel de peligrosidad de lo que envuelve.

### Agregados al camión
Se pide además, que se le pueda consultar al camión si tiene alguna cosa que pesa entre un valor mínimo y un valor máximo, y la cosa más pesada que tiene cargada.



### Tests hasta acá
Hay que hacer un pequeño test para cada una de las siguientes cosas: paquete de ladrillos, batería antiaérea, contenedor portuario y embalaje de seguridad. Al embalaje ponerle adentro los residuos radioactivos con 30 kg de peso. Al contenedor, dos o tres cosas a elección. .

Por otro lado, armar un test del camión, cargado con lo siguiente: bumblebee como robot, la arena a granel con 150 kilos, la batería antiaérea con los misiles puestos, y el embalaje de seguridad poniéndole como contenido el paquete de ladrillos con 80 ladrillos.  
Para cada método, calcular qué resultado tiene que dar, y hacer el test correspondiente.  


