**Medios de almacenamiento**

Sin importar qué [método de backup](BACKUP-Methods.md) se utilice, el backup se debe almacenar en algún medio de almacenamiento de datos, también conocido como el "destino" del backup.

**Cinta Magnética** (*Tape*)

Durante muchos años fueron el medio más utilizado para realizar backups, archivado de datos e intercambiar grandes cantidades de información. La cinta es un medio de acceso secuencial por lo que la velocidad de lecto-escritura continua (de datos contiguos) puede ser muy elevada.

Las capacidades típicas de las cintas actuales se encuentran en el orden de 15 a 20 GB, aunque hay fabricantes (*Fujifilm* y *Sony*) que anunciaron (en el año 2014) capacidades del orden de los 180 a 250 GB.

Entre los problemas de la cinta se destacan:

* La compatibilidad. Existen varios sistemas de tipos de cinta, incompatibles entre sí. Sin embargo, hoy día parece haber un estandar aceptado: [LTO](https://en.wikipedia.org/wiki/Linear_Tape-Open), con una durabilidad de entre 15 y 30 años.
* La confiabilidad. Las cintas se arruinan "con facilidad" y son sensibles a los campos magnéticos potentes, pudiendo borrarse por completo si son sometidas a dichos campos.
* El rendimiento de acceso aleatorio. Esto impactaría la restauración de archivos selectiva ya que el medio tiene que ser "recorrido" de manera secuencial hasta encontrar los archivos en cuestión.
* El ruido. En general son muy ruidosos durante la restauración debido al ruido que generan los motores al rebobinar o avanzar las cintas en búsqueda de la información a restaurar.

**Almacenamiento Óptico** (*CD*, *DVD*, *Blu-Ray*)

El almacenamiento óptico utiliza lásers para escribir y leer la información. Los discos *CD*, *DVD* y *Blu-Ray* (re-)grabables son de uso común en computadoras personales y en general son baratos.

Al principio estos medios eran mucho más lentos que las cintas y que los discos rígidos, pero los avances tecnológicos acortaron la brecha.

La capacidad va desde 0.7GB (*CD*) a 25-128GB (*Blu-Ray* de una a cuatro capas).

Según un estudio de 2008 el tiempo de vida de los *CD* grabables (*CD-R*) vendidos típicamente era de 2 a 10 años, pero más tarde un fabricante estimó la longevidad de sus *CD-R* recubiertos en oro en más de 100 años. Para más información se puede consultar un [estudio del Gobierno de Canadá sobre la vida útil de distintos medios de almacenamiento óptico](https://www.canada.ca/en/conservation-institute/services/conservation-preservation-publications/canadian-conservation-institute-notes/longevity-recordable-cds-dvds.html) (en inglés).

**Disco Rígido**

El uso de los discos rígidos como medio de almacenamiento para los backups se popularizó en los últimos años debido a la reducción de los costos y al aumento de la capacidad de los mismos. Por lo general, los discos rígidos son de fácil uso, es muy fácil conseguirlos, y son de fácil acceso.

Sin embargo, cabe recordar que los discos rígidos son dispositivos mecánicos (con partes móviles) y que están sujetos al mismo tipo de fallas que los medios que contienen los datos que se intentan resguardar (el disco rígido de nuestra computadora), y además corren riesgo de dañarse durante su transporte.

En los últimos años (2005-2015) los discos rígidos portátiles incluyen tecnologías (rampa de carga y acelerómetro) para minimizar (o anular por completo) los daños producidos por las caídas de los discos mientras no se encuentran en operación. Algunos discos rígidos portátiles (*rugged*) incluyen una funda de absorción de impactos.

**Almacenamiento de Estado Sólido** (*SSD*, *pendrive*, tarjetas *SD*, *CompactFlash*, etc.)

Los discos (o tarjetas de memoria) de estado sólido utilizan circuitos integrados (de memoria no volátil, tipo *flash*) para almacenar datos.

Los dispositivos de estado sólido son relativamente caros debido a su limitada capacidad (con respecto a los discos rígidos), pero son convenientes para almacenar cantidades limitadas de información en un espacio reducido y muy portátil.

Los dispositivos de estado sólido no tienen partes móviles, lo que los hace mas resistentes al daño físico (rotura por caídas por ejemplo) y pueden tener una tasa de transferencia de datos muy elevada, de hasta 6 Gbit/seg.

**Almacenamiento Remoto**

El almacenamiento remoto, o *en la nube*, implica que se contrata un proveedor de servicios de almacenamiento online. También se puede utilizar otro equipo en la red LAN con software adecuado para realizar almacenamiento "remoto"; no obstante aquí nos referimos al almacenamiento en la nube u *off-site*, en otro sitio apartado geográficamente y operado por un tercero.

Este medio de almacenamiento se usa para protegerse de desastres naturales como incendios, inundaciones o terremotos que pueden destruir los backups almacenados de manera local.

Sin embargo, se debe confiar en que el proveedor del servicio mantenga la privacidad y la integridad de nuestros datos. Se pueden usar soluciones de cifrado para mejorar la confidencialidad de la información. Otros factores a tener en cuenta son la velocidad y la disponibilidad, limitadas por la calidad de nuestra conexión de red (Internet), y el costo por GB.
