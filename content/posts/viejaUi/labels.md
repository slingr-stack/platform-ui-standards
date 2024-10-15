## **Labels**

Para los labels, hemos decidido modificar el comportamiento del responsive (wrappeo) para los HTML Tags. Si se llegase a hacer un ajuste a los labels por defecto, deberiamos alinearlos con estos cambios.

Le hemos agregado una mejoria para cortar los labels con la propiedad **word-break** setteada en **auto-phrase**. Esto se debe a que estabamos cortando las palabras para aprovechar espacio y no siendo concientes de la usabilidad de la misma. Respecto a grandes strings lo logico es poder ver toda la palabra en linea (por ejemplo un ID), asique este cambio se alinea con nuestra politica.