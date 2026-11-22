# WQ Files – Patches

La pestaña **Patches** se añade al diseño WQ Prism sin quitar Home, Apps, Clean ni Backups.

1. Seleccionar un archivo `.3105` o `.3106` desde el selector de documentos.
2. Introducir la ruta absoluta de un archivo existente al que WQ Files tenga acceso de escritura.
3. Confirmar el reemplazo. Se utiliza `wq_write_from_file_with_backup`, la API existente de WQ Files, para crear un respaldo antes de reemplazar.
4. Restaurar el original mediante la pestaña **Backups**.

No descubre automáticamente rutas de juegos ni elude permisos de iOS. Los patches son archivos de reemplazo completos; no se interpretan como instrucciones de modificación binaria. El acceso real depende de la versión de iOS, los permisos y el destino. El ZIP incluye código fuente; compilar la IPA requiere macOS con Xcode y las condiciones de `build.sh`.
