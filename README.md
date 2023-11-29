# closure13k.github.io

#### Posteriormente esto será convertido en sitio web.
El contenido se moverá a [este sitio web](https://closure13k.github.io/)

---

## Inicio de investigaciones (sin script)
<br>

Crear carpeta con nombre, fecha y hora
```bash
echo "Nombre para el archivo: " && read nombreArchivo && mkdir ~/Downloads/$nombreArchivo-$(date +%Y%m%d_%H%M%S)
```
Crear carpeta con nombre, fecha y hora y cambiar a ella
```bash
echo "Nombre para el archivo: " && read nombreArchivo && combinedValue="$nombreArchivo-$(date +%Y%m%d_%H%M%S)" && mkdir -p ~/Downloads/"$combinedValue" && cd ~/Downloads/$combinedValue
```
<br>

---

## Metagoofil
<br>
Para una descarga simple de n archivos de un dominio:
<br>

```bash
metagoofil.py -d <dominio> -t <tipo_archivo> -n 100 -o <directorio_descarga> -w
```

```bash
uso: metagoofil.py [-h] -d DOMINIO [-e RETARDO] [-f [ARCHIVO_GUARDAR]]
                   [-i TIMEOUT_URL] [-l BUSQUEDA_MAX] [-n LIMITE_DESCARGA_ARCHIVOS]
                   [-o DIRECTORIO_GUARDAR] [-r NUMERO_HILOS] -t TIPOS_ARCHIVOS
                   [-u [AGENTE_USUARIO]] [-w]

Metagoofil v1.2.0 - Busca en Google y descarga tipos de archivos específicos.

opciones:
  -h, --ayuda           muestra este mensaje de ayuda y sale
  -d DOMINIO            Dominio a buscar.
  -e RETARDO            Retardo (en segundos) entre búsquedas. Si es demasiado
                        pequeño, Google puede bloquear tu IP; si es demasiado
                        grande, la búsqueda puede tardar mucho. Predeterminado: 30.0
  -f [ARCHIVO_GUARDAR]  Guarda los enlaces html en un archivo.
                        no -f = No guardar enlaces
                        -f = Guardar enlaces en html_links_<MARCA_DE_TIEMPO>.txt
                        -f ARCHIVO_GUARDAR = Guardar enlaces en ARCHIVO_GUARDAR
  -i TIMEOUT_URL       Número de segundos para esperar antes de que expire el
                        tiempo de espera para páginas inaccesibles/anticuadas. Predeterminado: 15
  -l BUSQUEDA_MAX       Resultados máximos a buscar. Predeterminado: 100
  -n LIMITE_DESCARGA_ARCHIVOS
                        Número máximo de archivos a descargar por tipo de archivo.
                        Predeterminado: 100
  -o DIRECTORIO_GUARDAR Directorio para guardar archivos descargados. El valor predeterminado es el directorio de trabajo actual, "."
  -r NUMERO_HILOS       Número de hilos de descarga. Predeterminado: 8
  -t TIPOS_ARCHIVOS     Tipos de archivos para descargar
                        (pdf,doc,xls,ppt,odp,ods,docx,xlsx,pptx). Para buscar
                        todas las 17,576 extensiones de archivo de tres letras, escribe "ALL"
  -u [AGENTE_USUARIO]   User-Agent para la recuperación de archivos contra el dominio -d.
                        no -u = "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)"
                        -u = User-Agent aleatorio
                        -u "Mi agente de usuario personalizado 2.0" = Tu User-Agent personalizado
  -w                    Descargar los archivos en lugar de solo ver los resultados de la búsqueda.

```
