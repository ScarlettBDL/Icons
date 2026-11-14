# Iconos

PNG blancos de 96×96 (Material Design) que usa `projects/ytmusic/Yt_v7_out (4).txt`.

## Estructura

```
icons/<categoría>/<nombre>.png
```

- `action/`: explore, favorite, home, search, settings, subject, translate, visibility, visibility_off
- `av/`: library_music, pause, play_arrow, repeat, repeat_one, shuffle, skip_next, skip_previous
- `content/`: add, remove
- `editor/`: drag_handle
- `image/`: edit
- `navigation/`: arrow_back, close, menu

## Cómo los usa el script

Al iniciar, `UI.Icons.start()`:

1. Busca cada PNG en `YTM_Data/icons/<nombre>.png`.
2. Si existe y es válido, lo registra con `getcustomasset` y **no lo descarga**.
3. Si falta o está dañado, lo baja desde:
   `https://raw.githubusercontent.com/ScarlettBDL/Icons/main/icons/<categoría>/<nombre>.png`
   y lo guarda en la caché local.
4. Si GitHub no está disponible y los recursos ya están en caché, el reproductor arranca igual.
   Si tampoco hay caché, se usan los glifos dibujados como respaldo.

## Origen y licencia

Iconos de [google/material-design-icons](https://github.com/google/material-design-icons),
Apache License 2.0. Se redistribuyen en blanco (grayscale + alpha).
