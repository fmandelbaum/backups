**Métodos de backup**

**No estructurado**

Puede ser simplemente un conjunto de cintas, DVD, discos rígidos, u otro medio con información mínima sobre qué se respaldó y cuando. Este método es el más fácil de implementar, pero el menos confiable a la hora de restaurar porque no se tiene información acerca de qué contienen las copias ni de cuándo fueron hechas.

**Completo**

Se realiza una copia de *todos* los archivos independientemente de qué archivos se crearon o cambiaron desde la última copia.

Una variante de este método es la *Imagen del sistema* donde se utiliza una herramienta para generar una "imagen" de una partición del disco o del disco completo. Sin embargo, esto se utiliza más para replicar sistemas idénticos de manera más sencilla, por ejemplo: se instala y configura todo el software necesario en una computadora, se realiza la imagen, y después se restaura la imagen en todas las computadoras necesarias.

El espacio de almacenamiento necesario es el de todos los archivos cada vez que se realiza la copia. Ejemplo: si se deben realizar tres respaldos de 10GB de archivos, se necesitan 30GB.

**Incremental**

Se copian *solo los archivos que cambiaron desde un punto de referencia en el tiempo*. No se copian archivos duplicados, o archivos que no cambiaron. Típicamente se realiza primero un backup *Completo* de los archivos que se utiliza como "referencia" para los backups incrementales, y luego se van realizando backups incrementales a intervalos regulares. Para restaurar los archivos se necesitan la copia completa más reciente y todas las copias incrementales intermedias.

Algunos sistemas (como el *Time Machine* de Apple Inc.) permiten sintetizar backups completos a partir de un conjunto de copias incrementales automáticamente, brindando así la "ilusión" de tener varias copias completas.

Este método necesita menos espacio de almacenamiento para la copia que el método *Completo*. Ejemplo: si se deben realizar tres respaldos de 10GB de archivos, pero entre el primero y el segundo sólo cambiaron o se crearon 1GB, y entre el segundo y el tercero sólo cambiaron o se crearon 3GB, sólo se necesitan 14GB, en lugar de 30GB.

**Diferencial**

Se copian *solo los archivos que cambiaron o se crearon desde el último backup completo*. Esto implica que para restaurar un sistema solo se necesitan dos copias, el último backup *Completo* y su backup *Diferencial*.

Sin embargo, a medida que transcurre el tiempo desde el último backup *Completo*, y los cambios en los archivos se van incrementando, también se incrementará el tiempo necesario para realizar el backup *Diferencial*.

Un backup *Diferencial* copia los archivos que se crearon o cambiaron desde el último backup *Completo*, sin importar si se hicieron otros backups diferenciales "en el medio"; mientras que un backup *Incremental* copia los archivos que se crearon o cambiaron desde el último backup de cualquier tipo (ya sea *Completo* o *Incremental*). Por lo tanto, el método *Diferencial* necesita menos espacio que el *Completo*, pero más que el *Incremental*.
