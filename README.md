Trasleate Spanish 
Video Tutorial
https://www.youtube.com/watch?v=-zfWllu2gy0
Versión actual 2.1.1

Esta plantilla trabaja con la mayoría de los lanzadores ... Pero es una plantilla y usted debe probar de forma individual antes de hacer afirmaciones para apoyar cualquier lanzador específico !

Gracias por usar mi fuente de su base de pack de iconos ... Espero que esto le ayuda a crear un paquete de iconos completa para varios lanzadores ... He dejado comentado líneas a través de los archivos ... Siéntase libre de leer para tener una mejor comprensión del código y lo que lo ! Algunas cosas tienen que cambiar ... Así que por favor siga leyendo y, al menos, hacer estas cosas PRIMERO !

REQUISITOS: algunos conocimientos básicos de código (yo explico mucho que hacer más fácil para no0bs ), también un conocimiento básico de paquetes de icono y cómo funcionan en términos de los archivos que necesita para editar / añadir es decir : conocer estos archivos esenciales deben ser actualizado para que coincida con sus propios iconos necesita appfilter.xml , icon_pack.xml , drawable.xml ... he incluido mis propios archivos de cada uno , que son grandes bases para empezar.

Paso 1: Descargar ActionBarSherlock ( se conoce como ABS a partir de ahora ) , si aún no lo ha hecho todavía https://github.com/JakeWharton/ActionBarSherlock

Paso 2: Importar este proyecto , ABS . A continuación, añadir ABS to Icon paquete de plantillas como su biblioteca dependiente. ( Importación de Eclipse - Haga clic derecho sobre la carpeta de plantillas y seleccione Propiedades> Android > Seleccionar 4.2.2 > Bajo eso, quitar cualquier importaciones malas y añadir ABS > Aplicar> Aceptar )

Paso 3 : . Abierto AndroidManifest.xml y cambiar la línea 22 A continuación, lea el comentario comienza en la línea 54 Usted puede experimentar con esas dos actividades en función de cómo desea que la aplicación se vea . . Siguiente desplácese hasta el fondo a la línea 157 y cambiar esa parte para que coincida con el nombre del paquete. Ya hemos acabado con el AndroidManifest.xml ahora se puede cerrar esta .

Paso 4 : Abra el directorio " src" y encontrar el paquete " your.icons.name.here " . Refractores que para que coincida con su propio nombre de paquete. Usted no debería, pero en caso de fallos en algunos de sus archivos java , tendrá que fijar las importaciones sobre los archivos que muestran un error.

Ahora comienza la diversión : D

Paso 5 : En función de cómo configure su base determinado en el paso 3 la línea 54 de su referenciación AndroidManifest.xml , determinará lo que se edita el próximo . Si usted lo dejó solo, navegue hasta el src > paquete gridview y abrir Main.java también navegar hasta src > adaptadores y MainAdapter.java abierto. O Si ha cambiado esa línea en el AndroidManifest.xml para android : name = " your.icons.name.here.AppActivity " a continuación, vaya al paquete your.icons.name.here y AppActivity.java abierto. En cualquier caso, todos los archivos se han comentado lo suficientemente bien para que usted entienda exactamente lo que necesita para editar . Si no se realizan estos cambios se traducirá en una aplicación que es casi idéntica a la de mi propia aplicación . Con enlaces a mis perfiles y aplicaciones en lugar de la suya .

Paso 6 : Navegue a res > Valores > strings.xml leer los comentarios allí y realice las modificaciones necesarias .

Paso 7 : Vaya a res> Valores > colors.xml puede editar estos o dejarlos solos cómo mejor le parezca. Aquí es donde usted va a invertir la mayor parte de la aplicación, si usted quiere y editar los colores de pieles temáticos como el color del texto , etc

! Ya casi está !

Paso 8: Navegue a res > estirable - nodpi y editar las vistas previas de fondo de pantalla y de imagen.

Paso 9: Navegue a res> mipmap - IPAP y mapas MIP - xhdpi y editar esa imagen con su cuenta o dejar mi cara bonita allí : D

Paso 10 : Añade tus propios iconos con el tamaño de 144x144px a los res > carpeta estirable - xxhdpi . Usted puede utilizar otros tamaños si quieres, de agregar a las otras carpetas también. Pero aquí es donde me pongo la mía.

Paso 11: Si usted NO desea invertir esta aplicación o cambiar de color , pasar al siguiente paso ... Todos los demás , vaya de nuevo a res> Valores > colors.xml ... Aquí es donde puede cambiar todas sus aplicaciones y fondos colores de texto ... Ir al siguiente paso si usted está utilizando el flatview mira ... Por listview, sólo un par de cosas más para editar ... a continuación, desplácese a la res> diseño > file listview_layout.xml ... Leer el comentario en la línea 27 .

Paso 12: Ahora, con su mirada invertida / normal de acabado, sus iconos añadió , sus nombres y descripciones cambiado, imágenes misceláneos editados ... creo que haya terminado ... es la Exportación y empezar a compartir con el mundo !

Cualesquiera otras ediciones a esto son totalmente suya ... Espero que te das cuenta de que una gran cantidad de tiempo que pasó en esto para no sólo hacer más fácil para usted para hacer un pack de iconos , pero para que entiendan realmente los cambios de código que están haciendo aquí ... Por favor, considere compartir esta información con cualquier persona que quiere hacer su propio paquete de iconos ...

También estoy buscando para algunas personas que deseen colaborar con el código ... Hay algunas cosas que podemos añadir a esto para hacerlo mejor! Si usted desea contribuir , mándame un email the1dynasty.android @ gmail.com Estoy seguro que todos agradecerá su contribución también!
