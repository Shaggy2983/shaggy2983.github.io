# shaggy2983.github.io

Raíz del dominio `shaggy2983.github.io`. Sólo sirve para dos cosas:

- **`.well-known/assetlinks.json`**: la verificación que Android exige
  para que la app **COORDINATE · Obra** (`com.coordinate.visorobra`) se
  abra a pantalla completa, sin barra de direcciones. Tiene que estar en
  la raíz del dominio; por eso no vale el del repositorio `Visor-de-obra`.
- **`index.html`**: redirige a la app, en `/Visor-de-obra/visita.html`.

## Huellas

`sha256_cert_fingerprints` lleva la huella SHA-256 de cada clave con la
que se firma la app:

| Clave | Huella | Dónde se ve |
|---|---|---|
| Subida (APK instalado a mano) | `D2:B5:23:55:…:FC:7E:9F` | Registro de «Compilar app Android», paso «Huella de la clave» |
| Firma de Google Play | *pendiente* | Play Console → Configuración → Integridad de la app → Firma de apps |

Cuando la app esté en Play, hay que **añadir** la huella de Google Play a
la lista (sin quitar la de subida). `.nojekyll` hace que GitHub Pages
sirva la carpeta `.well-known`.
