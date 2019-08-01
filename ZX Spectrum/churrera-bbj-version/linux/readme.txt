Utilidades

gentileset.sh
 * sprite convert: A partir de work.png y font.png crea el fichero que necesita la churrera (udgs+font)
 * uso: llámalo desde el directorio "dev" (ya está incluido en el make.sh, no tienes que llamarlo desde fuera si no quieres).

posterizeZX
 * convierte un png a colores de speccy normalizados, exactos a los que necesita gfxcnv.
 * posterizezx imgpsd.png imgspc.png

png2rcs
 * Convierte una imagen png a screen RCS (comprimida). Requiere colores exactos y se puede descomprimir con rcs -d.
 * uso: png2rcs loading.png loading.rcs

gfxcnv
 * a partir de font.png + work.png + sprites.png genera tileset.h y sprites.h, requiere colores exactos.
 * uso: gfxcnv font.png work.png sprites.png tileset.h sprites.h

tmxcnv
 * a partir del TMX de Tiled genera los ficheros para la churrera mapa.h y enems.h (ya está incluido en el make.sh)
 * tmxcnv ../map/mapa.tmx ../dev/mapa.h ../dev/enems.h

tmxcompress
 * a partir de un TMX de Tiled te permite usar un mapa comprimido. Necesita muchos cambios en la churrera, mejor no usarlo.
 * tmxcompress ../map/mapa.tmx ../dev/mapa.bin

map2tmx
 * Genera un mapa nuevo para usar en Tiled compatible con la churrera, también se puede usar para convertir viejos mapas.
            // <mapa_ancho> <mapa_alto> <tiles_ancho> <tiles_alto> <tile_cerrojo> <fichero_salida>
 * uso: map2tmx 5 4 15 10 15 mapa.tmx


######################################

Tiled

* activar ajustar a rejilla, para que los sprites se ajusten al tile. Pulsa en Colocar patrón (T), para colocar los enemigos.
* Poner los enemigos por orden o numerarlos en name correlativamente. Si numeras empieza a partir del 100.
* Usar type para la velocidad 1, 2, 4. Si no pone nada será 1.
* Para enemigos extra usa el sprite primero del enemigo 3 y en name ponle su tipo (ej: 7 para los murciélagos)


