# Photographs — image guidelines

Photos of the assembled board stack and of the system in a loudspeaker
environment go in this folder. Keep them to the spec below so the gallery stays
consistent with the project's other repositories.

## Format

| Property      | Value                                                                 |
|---------------|-----------------------------------------------------------------------|
| Aspect ratio  | **16:9**, landscape                                                   |
| Size          | **1600 × 900 px** (long edge 1600 px). Smaller is fine; never upscale. |
| File format   | **WebP**, quality ~80 (JPEG also acceptable)                          |
| File size     | Aim well under ~500 KB per image                                      |
| Colour space  | sRGB                                                                   |

## Naming

```
descriptive-slug_c_Photographer-Name.webp
```

- Lowercase, hyphen-separated slug describing the shot.
- `_c_` marks the credit, followed by the photographer's name with underscores.
- Example: `board-stack-detail_c_Lorenz_Schwarz.webp`

## Embedding in the README

Photos are single images (no light/dark variants — those are only for the SVG
diagrams). Centre the image and follow it with an italic caption and credit:

```html
<p align="center">
  <img alt="Assembled LFSR board stack" src="assets/img/photos/board-stack_c_Photographer.webp" width="640">
</p>
```

*Caption text. Photo: © Photographer.*

## Note on diagrams vs. photos

- **Diagrams** (in `assets/img/diagrams/`) ship as **light/dark SVG pairs** and are
  embedded with `<picture>` + `prefers-color-scheme`.
- **Photos** (this folder) are a **single raster image** at the 16:9 spec above.
