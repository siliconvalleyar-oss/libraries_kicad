# KiCad Libraries

Librerías personalizadas para KiCad organizadas en tres categorías:

## Estructura

```
libraries_kicad/
├── symbols.kicad_sym      # Librería de símbolos (45 componentes)
├── footprints.pretty/      # Librería de footprints (75 patrones)
├── 3dmodels/              # Modelos 3D (14 modelos STEP)
└── .gitignore
```

## Librerías

### Símbolos (`symbols.kicad_sym`)

Componentes electrónicos para esquemáticos:

| Categoría | Componentes |
|-----------|-------------|
| ICs | 74HCT245D, DS2482S-100, LPCXPRESSO_LPC1769, PIC18F4620-E_P, SN75451BP |
| Módulos | MRF24J40MA, Raspberry Pi Pico, Raspberry Pi Pico W |
| Sensores | ALS31300EEJASR-500, HFBR-1531, HFBR-2531Z |
| Conectores | F31L-1A7H1-11024, F32R-1A7H1-11024, PIM100 |
| Alimentación | BAT-HLD-012-SMT, VI-264-EU-F2 |
| Memoria | M48T08-100PC1 |
| Diodos | SS34 |

### Footprints (`footprints.pretty/`)

Patrones de pads para PCB:

- **SMD**: SOIC, QFN, DFN, SOT, QFP, DIP
- **Conectores**: Pin headers, USB, Barrel Jack
- **Pasivos**: 0603, 0805, 1206, 2512
- **Especiales**: Raspberry Pi, displays, oscillators

### Modelos 3D (`3dmodels/`)

Modelos STEP para visualización en PCB:

- 74HCT245D, ALS31300EEJASR-500, BAT-HLD-012-SMT
- DS2482S-100, F31L-1A7H1-11024, F32R-1A7H1-11024
- HFBR-2531Z, M48T08-100PC1, PIC18F4620-E_P
- Raspberry Pi Pico, Raspberry Pi Pico W, SS34
- VI-264-EU-F2, SN75451BP

## Instalación en KiCad

### Símbolos
1. Copiar `symbols.kicad_sym` a `~/Documents/KiCad/symbols/`
2. En KiCad: Pref Preferences → Manage Symbol Libraries
3. Agregar nueva librería y seleccionar el archivo

### Footprints
1. Copiar la carpeta `footprints.pretty/` a `~/Documents/KiCad/footprints/`
2. En KiCad: Pref Preferences → Manage Footprint Libraries
3. Agregar nueva librería y seleccionar la carpeta

### Modelos 3D
1. Copiar archivos `.step` a `~/Documents/KiCad/3dmodels/`
2. Los modelos se asignan automáticamente a los footprints correspondientes

## Contribuir

1. Fork el repositorio
2. Crear branch (`git checkout -b feature/nuevo-componente`)
3. Commit (`git commit -m 'Agregar componente X'`)
4. Push (`git push origin feature/nuevo-componente`)
5. Abrir Pull Request

## Licencia

Librerías bajo licencia GPL v2+ (compatible con KiCad)

## Autor

**siliconvalleyar-oss** - siliconvalleyar@gmail.com

## Changelog

### v1.0.0
- Versión inicial con 45 símbolos, 75 footprints y 14 modelos 3D
- Eliminación de duplicados entre librerías
- Organización en estructura limpia
