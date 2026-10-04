# Política de Privacidad de GeoSweeper

**Fecha de entrada en vigor:** 26 de septiembre de 2026

**Última actualización:** 4 de octubre de 2026

## La versión resumida

GeoSweeper no recopila, transmite, vende ni comparte ninguna información personal. Cada
tablero que juegas, cada ajuste que eliges y cada país que has completado se almacena
únicamente en tu dispositivo. Nada se sube a nuestros servidores, y no existe ninguna cuenta
que crear en primer lugar. El único tráfico de red que GeoSweeper genera es StoreKit
comunicándose con Apple cuando haces o restauras una compra, y las páginas que abres
deliberadamente desde un enlace dentro de la app (este sitio, o las propias páginas legales de
Apple) — ambos casos se explican más abajo, y ninguno de los dos lleva consigo nada más.

## Quiénes somos

GeoSweeper está desarrollada por Ivan Cayabyab. Las preguntas sobre esta política o sobre la
app pueden enviarse a ivnsjdev@gmail.com.

## Qué almacena la app, y dónde

Todo lo que se describe a continuación vive únicamente en tu dispositivo, en uno de tres
lugares: `UserDefaults` (valores de ajustes pequeños), un archivo JSON en la carpeta de
Application Support propia de la app, o una base de datos SQLite local.

| Qué | Almacenamiento principal | ¿Se nos envía automáticamente? |
|---|---|---|
| Ajustes de visualización — tema del tablero, color neón, efecto de explosión, sonido de impacto, proyección del mapa (**Globe** o **Flat**), sonido y hápticos activados/desactivados | `UserDefaults` | No |
| Idioma que has elegido dentro de la app | `UserDefaults` | No |
| Registro del aviso de valoración — las fechas en las que GeoSweeper le ha pedido a iOS que muestre la hoja de valoración nativa, y qué hito desencadenó la última | `UserDefaults` | No |
| Contadores de partidas gratuitas — cuántos de tus 10 países gratuitos del mapa y tus 10 partidas gratuitas de **Classic** has usado | `UserDefaults` | No |
| Registro por país — victorias, derrotas, mejor tiempo, y cuándo lo desbloqueaste, para cada país que has jugado | Un archivo JSON (`progress.json`) en la carpeta Application Support de la app | No |
| Historial del modo **Classic** — el tamaño del tablero, la dificultad, el número de minas, el tiempo y la victoria o derrota de cada partida de Classic terminada | Un archivo JSON (`Classic/history.json`) en la carpeta Application Support de la app | No |
| Progreso de **Infinite Tower** — la fila a la que has llegado, tu vista guardada, y qué filas has despejado | Una base de datos SQLite local | No |

Nada de esto se transmite, se vende ni se comparte con nadie, incluidos nosotros. El propio
tráfico de StoreKit (más abajo) y los enlaces externos que toques (también más abajo) no
llevan consigo nada de esto. Una copia de seguridad del dispositivo iOS puede incluir estos
archivos como parte de la copia de seguridad de la app en su conjunto — esa copia la inicias
tú o iOS, nunca GeoSweeper, y permanece donde tú la envíes (iCloud o tu ordenador), no con
nosotros.

## Sin cuenta, sin inicio de sesión, sin nube

GeoSweeper nunca pide un nombre, una dirección de correo electrónico, un número de teléfono,
una fecha de nacimiento ni ningún otro dato identificativo — no hay nada con lo que iniciar
sesión, porque no hay cuenta. Tu progreso no se sincroniza mediante iCloud, CloudKit ni ningún
otro servicio: vive únicamente en el dispositivo en el que estás jugando. Juega el mismo país
en un segundo dispositivo y empezará desde cero allí, porque no hay ninguna copia en un
servidor desde la que sincronizar.

## Algo que deliberadamente no se guarda

El tablero en el que estás a mitad de partida — cada casilla que has abierto, cada bandera que
has colocado — se mantiene solo en memoria mientras juegas. Esto vale para los tres mundos: el
mapa, el modo **Classic** e **Infinite Tower**. Cierra la app a mitad de partida y ese tablero
desaparece; nunca se escribe en disco, y no hay autoguardado desde el que retomar un tablero
sin terminar. Solo una partida *terminada* (una victoria o una derrota) actualiza el registro
por país o el historial de Classic descritos arriba.

## Lo único que parece que no es local

El mapa se abre en tu propio país la primera vez que inicias la app. Esto proviene del
**ajuste de región** de tu dispositivo (el país vinculado a tu idioma y configuración regional,
el mismo que usa iOS para elegir un teclado y un calendario) — no del GPS, del Wi-Fi ni de
ninguna otra forma de seguimiento de ubicación. GeoSweeper no solicita acceso a la ubicación y
no podría leer tus coordenadas aunque quisiera.

## Permisos

GeoSweeper no solicita ningún permiso del sistema. Nunca pide acceso a la cámara, la
biblioteca de fotos, el micrófono, la ubicación, los contactos, el calendario, los datos de
salud, los datos de movimiento ni las notificaciones push, y nunca aparecerá ningún aviso de
permiso de ningún tipo. Esto coincide exactamente con el `Info.plist` de la app: no hay ni una
sola entrada de descripción de uso en él.

## Compras

GeoSweeper es gratis de descargar, y cada uno de sus tres mundos tiene su propia prueba
gratuita. Tus primeros 10 países del mapa — de cualquier nivel, incluido **Beginner** — son
gratis de jugar, y una vez que has jugado un país queda disponible para siempre, incluso
después de agotar esa prueba. El modo **Classic** te da 10 partidas gratuitas de la misma
forma. **Infinite Tower** es gratis hasta la fila 10. Más allá de esos puntos, hay tres
compras independientes, todas de pago único, no consumibles, y ofrecidas a través de StoreKit
de Apple y procesadas íntegramente por Apple:

- **All Countries** — una compra de pago único y no consumible que desbloquea de forma
  permanente los niveles **Intermediate**, **Expert** y **Mega** en los 204 países. Nada de
  esto se renueva.
- **Classic Lifetime** — una compra de pago único y no consumible que desbloquea de forma
  permanente las partidas ilimitadas de Classic una vez agotadas tus 10 gratuitas. Nada de
  esto se renueva.
- **Infinite Tower Lifetime** — una compra de pago único y no consumible que desbloquea de
  forma permanente subir más allá de la fila 10. Esto tampoco se renueva, y GeoSweeper no
  ofrece ningún tipo de suscripción.

Apple, no GeoSweeper, procesa cada pago. Ningún número de tarjeta, dirección de facturación ni
credencial de tu cuenta de Apple es visible para nosotros nunca — StoreKit solo le dice a la
app lo que necesita para mostrar una pantalla de compra y conceder el acceso: el precio que
mostrar, y si ya eres propietario de cada artículo. Esas respuestas permanecen en tu
dispositivo; GeoSweeper no gestiona ningún servidor de compras propio y no tiene dónde
enviarlas. Restaurar compras le pide a Apple que reconfirme qué posee tu cuenta de Apple y
aplica la respuesta localmente — no crea ni transmite ningún registro nuevo.

Consulta también el documento de Apple [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/),
el [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/), y el
[Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), que rigen
la compra en sí.

## Comunicaciones de soporte

Si escribes a ivnsjdev@gmail.com, recibimos tu dirección de correo electrónico, lo que
escribas y cualquier archivo adjunto que decidas añadir. La usamos únicamente para
responderte y resolver el problema por el que escribiste — nuestra base legal es nuestro
interés legítimo en responder a quienes nos contactan. Ese buzón es una cuenta de Gmail
estándar, procesada por Google LLC según la
[Política de Privacidad de Google](https://policies.google.com/privacy), y alojada en
infraestructura que puede estar ubicada fuera de tu propio país, razón por la cual esa
transferencia se indica aquí. Conservamos los correos de soporte hasta 24 meses y luego los
eliminamos; puedes pedirnos que eliminemos un correo concreto antes escribiendo a la misma
dirección.

## Enlaces externos

Las pantallas de compra de GeoSweeper enlazan a la política de privacidad de este mismo sitio
y al Standard EULA de Apple; Settings puede enlazar a la página de escribir una reseña de la
App Store. Ningún dato de usuario ni identificador propio de la app se añade a ninguno de
estos enlaces — son URL simples, iguales para todo el mundo.

## Nada que apostar

GeoSweeper no tiene moneda dentro de la app, ni loot, ni sorteos, ni ninguna función en la
que un resultado se apueste o se arriesgue. Cada compra es un precio fijo y declarado por un
acceso permanente o temporal a contenido; no hay nada que se pueda ganar, perder ni jugarse.

## Lo que NO hacemos

- Ningún tipo de análisis, informe de errores ni telemetría
- Ninguna publicidad, ninguna red publicitaria y ningún identificador publicitario
- Ningún seguimiento entre apps o sitios, y ningún bróker de datos
- Ninguna cuenta, ningún inicio de sesión, ninguna contraseña
- Ningún acceso a cámara, biblioteca de fotos, micrófono, contactos, ubicación precisa o
  aproximada, ni datos de salud
- Ningún entrenamiento de modelos de aprendizaje automático con tus datos
- Ningún SDK de terceros de ningún tipo — el único código de esta app es el nuestro

Esto coincide con la etiqueta **Data Not Collected (datos no recopilados)** que GeoSweeper
lleva en la App Store.

## Conservación y eliminación

Eliminar la app elimina todos los archivos que almacenó en tu dispositivo — ajustes, tu
registro por país, tu historial del modo Classic y tu progreso de Infinite Tower — de forma
inmediata y completa, porque
nunca hubo una copia en un servidor que nosotros pudiéramos conservar ni eliminar por nuestra
parte. Una copia de seguridad de iCloud hecha antes de la eliminación puede seguir
conteniendo una copia; esa copia de seguridad está completamente bajo tu control a través de
**Ajustes → tu nombre → iCloud → Administrar almacenamiento de la cuenta** en tu dispositivo.
Los correos de soporte se conservan y se eliminan por separado, como se describe arriba.

## Tus derechos

Como GeoSweeper no conserva ninguna copia de tus datos dentro de la app, los derechos de
acceso, corrección, exportación y eliminación que describen el RGPD, el RGPD del Reino Unido
y la CCPA/CPRA son derechos que ya ejerces directamente, en tu propio dispositivo — no hay
ningún registro aquí que nosotros podamos producir ni borrar en tu nombre. El único lugar
donde sí conservamos algo es un correo de soporte que nos hayas enviado, y puedes pedir
verlo, corregirlo o eliminarlo en cualquier momento escribiendo a ivnsjdev@gmail.com. No
vendemos ni compartimos información personal con fines de publicidad conductual entre
contextos, y nunca lo hemos hecho. Si crees que hemos gestionado mal tus datos, tienes
derecho a presentar una reclamación ante tu autoridad local de protección de datos.

## Menores

GeoSweeper lleva una clasificación de edad apta para un público general y no está dirigida
específicamente a menores. No recopilamos a sabiendas información personal de nadie,
incluidos los menores de 13 años, y no hay nada en la app que pudiera hacerlo — ni chat, ni
funciones para compartir, ni funciones sociales, ni publicidad, ni cuenta a través de la cual
un tercero pudiera contactar con un menor.

## Cambios en esta política

Si esta política cambia, la fecha de arriba cambiará con ella, y un cambio material en lo que
GeoSweeper hace con los datos también se indicará en las notas de la versión de esa
actualización.

## Contacto

ivnsjdev@gmail.com
