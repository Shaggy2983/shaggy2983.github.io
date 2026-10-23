# shaggy2983.github.io

Raíz del dominio `shaggy2983.github.io`. Sirve para dos cosas:

- **`.well-known/assetlinks.json`**: la verificación que Android exige
  para que la app **COORDINATE · Obra** (`com.coordinate.bitacora`) se
  abra a pantalla completa, sin barra de direcciones. Tiene que estar en
  la raíz del dominio; por eso no vale el del repositorio `Visor-de-obra`.
- **`index.html`**: portada pública de la app (qué hace, enlace a la app,
  a Google Play y a la política de privacidad, y para qué usa los permisos
  de Google). Es la «página principal» que pide la verificación de la app
  OAuth de Google; la app Android abre directamente `visita.html`.

## Huellas

`sha256_cert_fingerprints` lleva la huella SHA-256 de cada clave con la
que se firma la app:

| Clave | Huella | Dónde se ve |
|---|---|---|
| Subida (APK instalado a mano) | `D2:B5:23:55:…:FC:7E:9F` | Registro de «Compilar app Android», paso «Huella de la clave» |
| Firma de Google Play | `36:46:33:CC:…:AA:39:0B` | Play Console → Configuración → Integridad de la app → Firma de apps |

Las dos huellas tienen que seguir en la lista (la de subida, para el APK de
prueba instalado a mano). `.nojekyll` hace que GitHub Pages
sirva la carpeta `.well-known`.
