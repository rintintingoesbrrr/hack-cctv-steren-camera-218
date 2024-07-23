#camara stren cctv 218
##disasembly 
no hay ninguna spec sheet que nos diga datos de la camara por el momento 
podemos obtener informacion de la etiqueta en el bottom de la camara
tiene una etiqueta con 2 iconos, uno de la oprganizacion de certificacion y normalizacion NYCE
y otra de NOM
tiene un numero desconocido PO 41813 y una version 1.0
El numerod de po es para distinguir el producto en la base de datos de steren

eso es todo lo que encontramos a simple vista iniciaremos con el disassembly

en el fondo de la camara hay 3 gomas que parecen esconder 3 tornillos
al quitar la tapa del fondo encontramos lo que parece ser un motor y un controlodar para el motor, estos para que la camara peuda girar 
tambien podemos sacar el controlador para recibir poder por microusb

hay otros 2 tornillos sosteniendo el motor, pero primero quitare los que parecen agarrar a la camara
hay 2 tornillos que estan muy lejos para mi desatornillador

LETS GOOO
ENCONTRE UN DEASTORNILLADOR DESPUES DE UNA HROA QUE IS ENTRO
TENEMOS ACCESO A LA CAMARA

Adentor encontramos un chip ANYKA 
AK3918EN080
V330
BATJ01K21

La placa tiene un conector donde se alimenta y esta conectado a el modulo de microusb
2 conectores para el control de los servmotores
un conector para ina bocina
los 2 motores son identicos
la placa esta asegurada con 3 tornillos, el otro lado de la placa esta escondido y debo de sacarla para ver como esta conectada a la camara

del otro lado de la placa encontramos el sensor de luz y el enfoque 

tambien estan unidos a otro elemento que no se que es aun 
hipotesis actual se encarga de manejar la vision nocturna con focos infrarojos


en la parte que no esta escondida de la palca madre habia un chip escondido abajo de una etiqueta qr pequeña 
es un chip REALTEK 8188FTV
parece ser un chip para control wifi

tengo que catalogarlos todos para encontrar cual es el que maneja el control 
el principal contendiente es el ANIKA

hay otro chip que al parecer se encarga de la memoria es el Gigadevice 25Q64ESIG
a simple vista no veo algun pin que pueda ser parte del protocolo uart entonces tengoq ue usar el multimetro para encontrarlos 

##prueba de pins uart de izquierda a derecha los pines sera 1 2 3 4 iniciando por voltage y terminando en gnd 

el pin uno es voltaje 4 es gnd
el pin 3 fluctuo en voltaje al inicio, probablemnte sea su pin te tx y el pin 2 es de rx


