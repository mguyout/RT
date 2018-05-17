# RT
4e projet de la branche graphique du [cursus 42](https://www.42.fr).

Ce projet doit être complété par un groupe de 4 élèves.

## Description

L'objectif de ce projet est de générer des images de synthèse en se basant sur la méthode du Raytracing (lancer de rayon).

Ces images de synthèses représentent une scène. Cette dernière peut être observée depuis différent angles/positions, définie par des objets simples/complexes ainsi que d'un système de lumières.

## Options

- Raytracer classique : 4 objets (sphere, cylindre, cone, plan), lumière, multi-spot, brillance, ombre
- Lumière parallèle
- Reflexion (le % de réflexion peut être modifié dans le fichier de configuration)
- Objet composé : le cube
- Objets natifs: l'ellipse, la parabole
- Objets limités: découpe basique, rotation, découpe propre à chaque objets.
- Objets exotique: le torus
- Environnement UI : interface graphique simple, modification en temps réel, génération automatique des scènes
- Options : fichier de configuration, lmière ambiante (peut être modifié dans le fichier de configuration)
- Textures : Appliqué aux 4 objets simple, mise à l'échelle, offset, utilisation de la librairie SDL_image pour upload les fichiers (.bmp, .jpg, .png...)
- Perturbations : rayures, arc-en-ciel, woodgrains, ondulation, damier, variation du bruit de Perlin (simple, marbre, bois)
- Effet visuel classic : antialiasing, filtre sépia, filtre noir & blanc
- Effet visuel technique : multithread, screenshot intégré
- Autre : enregistrement vidéo intégré, musique

## Usage

```
$> make
$> ./RT file/file.rt
```

## Contrôles

<table width="100%">
  <thead>
  <tr>
    <td width="40%" height="60px" align="center" cellpadding="0">
      <strong>Description</strong>
    </td>
    <td width="10%" align="center" cellpadding="0">
      <span style="width:70px">&nbsp;</span><strong>Key(s)</strong><span style="width:50px">&nbsp;</span>
    </td>
  </tr>
  </thead>
<tbody>
  <tr>
    <td valign="top" height="30px">Quitter le programme</td>
    <td valign="top" align="center"><kbd>&nbsp;esc&nbsp;</kbd></td>
  </tr>
    <td valign="top" height="30px">Filtre Sepia</td>
    <td valign="top" align="center"><kbd>&nbsp;s&nbsp;</kbd> <kbd>&nbsp;m&nbsp;</kbd></td>
  </tr>
  </tr>
    <td valign="top" height="30px">Flitre noir & blanc</td>
    <td valign="top" align="center"><kbd>&nbsp;n&nbsp;</kbd> <kbd>&nbsp;m&nbsp;</kbd></td>
  </tr>
    <td valign="top" height="30px">Changer de fichier de configuration</td>
    <td valign="top" align="center">
      <kbd>&nbsp;1&nbsp;</kbd><kbd>&nbsp;2&nbsp;</kbd><kbd>&nbsp;3&nbsp;</kbd>            <kbd>&nbsp;4&nbsp;</kbd><kbd>&nbsp;5&nbsp;</kbd><kbd>&nbsp;6&nbsp;</kbd>
      <kbd>&nbsp;7&nbsp;</kbd><kbd>&nbsp;8&nbsp;</kbd><kbd>&nbsp;9&nbsp;</kbd>
    </td>
  </tr>
  </tr>
    <td valign="top" height="30px">Clic gauche sur un objet : déplacez l'axe X ou Y en déplacant la souris de gauche à droite & de haut en bas </td>
    <td align="center"><img src="./img/left-click.png" width="35" height="35" alt="left-click"><img src="./img/cursor.png" width="35" height="35" alt="cursor"></td>
  </tr>
  </tr>
    <td valign="top" height="30px">Clic droit sur un objet : utilisé la molette de soris pour faire varier l'axe Z </td>
    <td align="center"><img src="./img/left-click.png" width="35" height="35" alt="mouse"><img src="./img/mouse.png" width="35" height="35" alt="mouse"></td>
  </tr>
  </tr>
    <td valign="top" height="30px">Clic droit + mouvement de souris pour déplacer la direction de la caméra </td>
    <td align="center"><img src="./img/right-click.png" width="35" height="35" alt="right-click"></td>
  </tr>
  </tbody>
</table>

## Exemples imagés

### Reflexion
<img src="./img/reflexion1.png" width="800" height="600" alt="Reflexion 1">
<img src="./img/reflexion2.png" width="800" height="600" alt="Reflexion 2">

### Perturbation de couleurs
<img src="./img/perturbations1.png" width="800" height="600" alt="Perturbations 1">
<img src="./img/perturbations2.png" width="800" height="600" alt="Perturbations 2">

### Textures
<img src="./img/textures1.png" width="800" height="600" alt="Textures 1">
<img src="./img/textures2.png" width="800" height="600" alt="Textures 2">

### Torre
<img src="./img/torus.png" width="800" height="600" alt="Torus">

### Parabole
<img src="./img/hyperboloid.png" width="800" height="600" alt="Hyperboloid">

### Cube
<img src="./img/cube.png" width="800" height="600" alt="Cube">

### Objet limité
<img src="./img/limit-cyl.png" width="800" height="600" alt="Limit cylinder">
