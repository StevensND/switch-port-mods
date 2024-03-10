Si no puedes leer las instrucciones correctamente, descarga el archivo .zip

```
# (NEW) CameraSpeed: Velocidad de rotación de la cámara libre.
# (NEW) Speed: Velocidad a la que se mueve la cámara libre.
# (NEW)AutoHideUI: Oculta automáticamente la interfaz de la cámara libre
# (NEW) AnimationSmoothing: Suaviza el secuenciador entre fotogramas clave, hace un arco entre cada fotograma clave básicamente.
# (NEW) AnimationFadeout: Hace que el último fotograma clave se mueva más despacio hasta detenerse por completo.

[UltraCam]
TriggerWithController = On
AutoHideUI = On
CameraSpeed = 30
Speed = 5
AnimationSmoothing = 0.25
AnimationFadeout = On

# (NEW) FOV: Cambia el campo de visión para todo el juego, incluido el arco, zoom in, zoom out y mucho más.
# (NEW) MenuFPSLock: Bloquea los FPS de los menús del juego a tu gusto.
# (NEW) MovieFPS: Bloquea los FPS de las cinemáticas a 30, 60 o 120. SOLO USAR CON EL MOD DE CINEMÁTICAS A 60FPS O ESTAS SERÁN MÁS RÁPIDAS Y ESTARÁN DESINCRONIZADAS.
# (NEW) IsTimeSlower: Cuando esté activado, el tiempo se ralentizará según el valor en float de la velocidad del tiempo.
# (New) TimeSpeed: En 0.0 pausa el transcurso del tiempo en el juego. 1.0 es por defecto, 2.0 es 2x más rápido/lento, etc.
# (OLD) DisableFog: Elimina la neblina del juego.

[Features]
Fov = 50
MenuFPSLock = 30
MovieFPS = 30
DisableFog = On
TimeSpeed = 1.0
IsTimeSlower = Off

# (NEW) Resolution: La resolución ahora también hereda la relación de aspecto automáticamente (sin embargo la interfaz de usuario sigue estirada) <-- Sólo tienes que buscar en Google tu resolución con la relación de aspecto deseada.
# Mantén 1920x1080 como máximo si estás usando jugando en Switch. (1600x900) es el valor predeterminado.
# (NEW) ¡Cualquier límite de FPS, siéntete libre de ajustarlo a tu gusto, valores entre 20-480 y cualquier cosa en el medio! :).
# (NEW) Triple Buffer, antes estaba activado por defecto ahora es opcional, esto se debe a que estaba causando problemas si juegas en Switch. SI ERES USUARIO DE SWITCH, MANTENLO DESACTIVADO (OFF)
# (NEW) QualityImprovements: Elimina FSR y Resolución Dinámica.
# (NEW) RemoveDepthOfField + RemoveLensflare: Elima la profundidad de campo y los rayos de luz.
# (NEW) EmuScale = Coincide con la escala del emulador, debe dejarse en 1 (1x en el emulador) para obtener la mejor calidad. Este ajuste soluciona los problemas de skyisland y otros problemas causados por el escalado del emulador ...
# (NEW) ShadowResolution: Sombras hasta 8K. MANTENER A 1024 COMO MÁXIMO si estás jugando en Switch. A Ryujinx no le gusta mucho este valor por lo que 2048 es el máximo.
# (NEW) DisableFXAA: Elimina el FXAA interno.

# (IMPORTANTE) LA RESOLUCION DE LAS SOMBRAS Y LA RESOLUCIÓN POR ENCIMA DE 1080P REQUIEREN MEMORIA HEAP EXTENDIDA. LA RESOLUCIÓN MAXIMA QUE HE PROBADO Y FUNCIONA ES 8K con SOMBRAS DE 8K.

[Resolution]
MaxFramerate = 60
Width = 1920
Height = 1080
EmuScale = 1.0
ShadowResolution = 1024
RenderDistance = 25000
QualityImprovements = On
TripleBuffer = Off
RemoveDepthOfField = On
DisableFXAA = On
RemoveLensflare = On

# (NEW) OverrideHandheld_Resolution: En lugar de 720p utilizará la Anchura y Altura globales establecidas en la sección RESOLUCIÓN.
# (NEW) Establezca aquí la resolución de Handheld.

[Handheld]
OverrideHandheld_Resolution = Off
Width = 1280
Height = 720

# (NEW) Coresponde a la velocidad de rotación de la cámara del jugador. (MULTIPLICADOR), cuidado con la velocidad vertical, va demasiado rápido si excede de 1.5

[Gameplay]
Stick_Vertical_Speed = 1.0
Stick_Horizontal_Speed = 1.0

# Benchmark Index
# 0 - Kakariko
# 1 - Great Sky Island
# 2 - Lookout Landing
# 3 - Goron City
# 4 - Korok Forest (Usarlo únicamente cuando el Bosque de Korok esté explorado completamente)

[Benchmark]
Benchmark = 1

# (NEW) Esto permite ajustar manualmente determinadas asignaciones de memoria
# El objetivo principal es facilitar el merging de mods ROMFS.
# Se trata de un multiplicador directo de determinados heaps.
# Los heaps gráficos son realizados automáticamente por UltraCam.
# Por favor, asegúrate de que no tienes un archivo romfs/System/Heap que pueda interferir con UltraCam.

[Heaps]
RSDB = 1.0
GameTextures = 1.0
```