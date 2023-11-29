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
