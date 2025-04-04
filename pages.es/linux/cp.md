# cp

> Copia archivos y directorios.
> Más información: <https://www.gnu.org/software/coreutils/manual/html_node/cp-invocation.html>.

- Copia un archivo a otro directorio:

`cp {{ruta/al/archivo_origen.ext}} {{ruta/al/archivo_destino.ext}}`

- Copia un archivo en otro directorio, conservando el nombre del archivo:

`cp {{path/to/archivo_origen.ext}} {{ruta/al/directorio_principal}}`

- Copia de forma recursiva el contenido de un directorio a otra ubicación (si el destino existe, el directorio es copiado en esa ubicación):

`cp {{[-r|--recursive]}} {{ruta/al/directorio_origen}} {{ruta/al/directorio_destino}}`

- Copia un directorio de forma recursiva en modo verbose (muestra los archivos a medida que se copian):

`cp {{[-vr|--verbose --recursive]}} {{ruta/al/directorio_origen}} {{ruta/al/directorio_destino}}`

- Copia varios archivos de inmediato a un directorio:

`cp {{[-t|--target-directory]}} {{ruta/al/directorio_destino}} {{ruta/al/archivo1 ruta/al/archivo2 ...}}`

- Copia todos los archivos con una extensión específica a otra ubicación en modo interactivo (pregunta al usuario antes de sobreescribir):

`cp {{[-i|--interactive]}} {{*.ext}} {{ruta/al/directorio_destino}}`

- Sigue los enlaces simbólicos antes de copiar:

`cp {{[-L|--dereference]}} {{link}} {{ruta/al/directorio_destino}}`

- Usa la ruta completa de los archivos de origen, creando los directorios intermedios faltantes al copiar:

`cp --parents {{ruta_de_origen/al/archivo}} {{ruta/al/archivo_destino}}`
