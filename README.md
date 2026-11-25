# Custodia — Descargas

Instaladores oficiales de **Custodia**, de Soluciones Integrales Mercasoft: respaldos automáticos de las
empresas CONTPAQi (SQL Server, ADD y sistemas no SQL) en una carpeta local y en OneDrive, cifrados y con
reporte por correo.

Este repositorio solo contiene las versiones publicadas. El código fuente no es público.

## Descargar

Descargue la última versión desde **[Releases → Latest](https://github.com/UNRGC/CUSTODIA-RELEASES/releases/latest)**:
el archivo `CustodiaSetup-X.Y.exe` de la sección *Assets*.

## Requisitos

- Windows 10 u 11, o Windows Server, de 64 bits.
- Permisos de administrador para instalar y abrir la aplicación.
- Acceso al SQL Server donde viven las empresas.
- Una licencia de Custodia vigente y conexión a internet para validarla.
- No requiere instalar .NET: el instalador lo incluye.

## Instalar

1. Ejecute `CustodiaSetup-X.Y.exe` como administrador y siga el asistente.
2. Abra **Custodia** desde el menú Inicio.
3. En **Información**, valide su número de serie.
4. En **Configuración**, capture los datos de SQL Server, genere la clave de cifrado y, si lo desea,
   conecte OneDrive.

## Actualizar

Desde la versión 1.8, la aplicación se actualiza sola: en **Información**, pulse el botón
**Buscar actualización**. Si hay una versión nueva, la descarga, comprueba que el archivo esté íntegro y la
instala. La aplicación se cierra y se vuelve a abrir al terminar. La configuración, las licencias y los
respaldos se conservan.

- Las versiones anteriores a la 1.8 se actualizan una vez de forma manual: descargue e instale la última
  versión encima de la actual; no hace falta desinstalar.
- Al actualizar se detiene el servicio por unos momentos; los respaldos o restauraciones en curso se
  interrumpen. La aplicación avisa antes si hay alguno.

## Verificar la descarga (opcional)

Cada archivo de *Assets* muestra su huella SHA-256. Para compararla con la del archivo descargado, en
PowerShell:

```powershell
Get-FileHash .\CustodiaSetup-X.Y.exe -Algorithm SHA256
```

## Soporte

Para dudas, licencias o problemas, contacte a Soluciones Integrales Mercasoft o a su distribuidor.
