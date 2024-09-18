# Visor 3D
Visor 3D embebido en un sencillo codigo HTML para poder visualizar modelos 3D con un telefono celular, a traves de un código QR

Esta basado en https://github.com/ajhamdi/html_3dviewer

Se utiliza **ONLINE 3D VIEWER**  https://3dviewer.net/

Es un software open source bajo licencia MIT  https://github.com/kovacsv/Online3DViewer

Trabaja con varios formatos (3dm, 3ds, 3mf, amf, bim, brep, dae, fbx, fcstd, gltf, ifc, iges, step, stl, obj, off, ply, wrl.)

## Pasos para compartir un modelo 3D a traves de un codigo QR
1. Subir el archivo del modelo 3D a un servidor (por ejemplo GitHub)
2. Utilizar el siguiente codigo HTML
```
<iframe
width="250" height="250" style="border:1px solid #eeeeee;"
src="https://3dviewer.net/embed.html#model=URL_archivo$camera=200,400,500,255,255,255,0,1,0,45">
</iframe>
```
En **URL_archivo** completar con la URL de la ubicacion del archivo que queremos compartir.

Cabe mencionar que si utilizamos Github, es mejor utilizar la version "raw" del archivo por lo que el enlace tendría que ser asi
```
https://raw.githubusercontent.com/usuario/Proyecto/main/Carpeta/archivo.stl
```
El visor 3D permite configurar 2 parámetros:

**defaultcolor** = Color predeterminado del modelo

**backgroundcolor** = Color de fondo

Ambos se configuran con códigos de colores RGB

HTML de ejemplo
```
<iframe
width="250" height="250" style="border:1px solid #eeeeee;"
src="https://3dviewer.net/embed.html#model=https://raw.githubusercontent.com/andesfreedesign/Visor3D/main/Modelos/clementina.stl$defaultcolor=255,255,255$backgroundcolor=66,110,23">
</iframe>
```
3. Para crear el código QR utilicé el procesador de texto _Writer_ de LibreOffice
- Ir al menú Insertar >> Objeto OLE >> Código de Barras y QR

![capture](https://github.com/andesfreedesign/Visor3D/blob/main/QR's/writer.png)

4. Finalmente se inserta la imagen del código QR, lista para compartir...

![capture](https://github.com/andesfreedesign/Visor3D/blob/main/QR's/clementina.png)


