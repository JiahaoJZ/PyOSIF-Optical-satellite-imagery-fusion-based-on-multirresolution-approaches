# Para ejecutar los ficheros se debe de crear un entorno con las dependencias de los cuadernos
Este entorno se puede generar haciendo uso del fichero image_fusion.yml

## Uso
### Existen dos flujos de ejecución principales
 - Pansharpening
 Para realizar pansharpening, descarga las imágenes de Landsat 8 con  **Download_Landsat8_Images.ipynb**, y seguidamente ejecuta **Pansharpening.ipynb**
 - Fusión de imágenes multiespectrales
 Para fusionar imágenes multiespectrales, descarga las imágenes de Landsat 8 y Sentinel 2 con **Download_Landsat8_and_Sentinel2_Images.ipynb**, a continuación emplea el cuaderno **Resizing_Module.ipynb** para reescalar la imagen de Landsat al tamaño de Sentinel 2, y finalmente realiza la fusión con **Multispectral_Images_Fusion.ipynb**
