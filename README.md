# Cum sa faci SPRITE

## Operarea cu Maki Editor

1. Accesezi [link-ul](https://labs.mapbox.com/maki-icons/editor/).

2. Stergi setul de date din editor.

3. Incarci file-urile .svg sau file-ul .json in editor.

4. Descarci setul de icons din editor.


## Operarea cu spritezero

### Instalarea spritezero si spritezero-cli

**Intri in directoriul dorit si faci git clone**

```bash
git clone https://github.com/mapbox/spritezero.git
```

**In directoriul spritezero:**

Instalezi npm local:
```bash
npm install
```


Scapi de erori:
```bash
npm audit fix --force
```

Intri in root:
```bash
sudo su
```

Scapi definitiv de erori:
```bash
npm audit fix --force
```

Instalezi spritezero-cli:
```bash
npm install -g @mapbox/spritezero-cli
```

Iesi din root:
```bash
exit
```

### Operarea

In directoriul spritezero adaugi folderul ./svgs descarcat din maki editor.

Creezi sprite:
```bash
spritezero [output filename] [input directory]

  --retina      shorthand for --ratio=2
  --ratio=[n]   pixel ratio
  --unique      map identical images to multiple names
```

#### Link-uri utile

https://labs.mapbox.com/maki-icons/editor/

https://labs.mapbox.com/maki-icons/guidelines/

https://github.com/mapbox/spritezero
