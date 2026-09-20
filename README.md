# DLSS5 Tools

DLSS5 Autoupdater y DLSS5 Profile Manager para Windows 10/11 x64.

## Descargar

[Descargar la ultima version](https://github.com/Xemizo/DLSS5-Tools-Releases/releases/latest)

Para la primera instalacion, descarga el ZIP `DLSS5-Tools-vX.Y.Z-win-x64.zip`.
Extraelo y abre `DLSS5 Autoupdater.exe`. Conserva ambos ejecutables juntos.
Los EXE sueltos de la release estan destinados al actualizador automatico.

Quienes tengan una version anterior a 0.3.0 deben descargar este ZIP una vez
manualmente. Desde 0.3.0, ambos programas comprueban las actualizaciones al
arrancar, sin cuenta, inicio de sesion ni tokens de GitHub.

## Actualizaciones

Los paquetes se verifican por origen, version, tamano y SHA-256 antes de
activarse. Cada version se instala por separado en
`%LOCALAPPDATA%\DLSS5Tools`, conservando la anterior. Los mismos ejecutables
que extrajiste sirven de entrada para abrir las versiones posteriores.

Los perfiles, ajustes y cache existentes se conservan. Sin conexion o ante
un error de descarga se utiliza la version disponible. La comprobacion puede
cancelarse con `Abrir sin actualizar`.

DLSS 5 Swapper sigue actualizandose desde su repositorio oficial.

## Streamline y requisitos

El ZIP no incluye DLL de Streamline, modelos NVIDIA ni archivos de juegos. Al
aplicar un perfil OptiScaler con DLSSG, Profile Manager usa Streamline completo
del propio juego o la cache local. Si faltan los archivos, descarga Streamline
SDK 2.12.0 directamente de NVIDIA, comprueba su SHA-256 y muestra el progreso.
No reemplaza una instalacion completa; al reparar una carpeta incompleta,
conserva una copia de seguridad. `Guardar Streamline` sigue disponible para
importarlo manualmente desde otro juego.

Windows PowerShell 5.1 y .NET Framework 4.x. Los ejecutables no estan firmados
con Authenticode: Windows puede indicar que el editor es desconocido.
Las sumas de los archivos se publican en `checksums.sha256`.

## Seguridad

No introducir contrasenas ni tokens de GitHub en el programa. No adjuntar
perfiles personales, logs o rutas privadas al informar de un problema.
El codigo se mantiene en un repositorio privado; estas descargas son publicas.

DLSS5 Tools es independiente de DLSS 5 Swapper, NVIDIA, OptiScaler y ReShade.
Actualizar las herramientas no modifica los archivos de los juegos.
