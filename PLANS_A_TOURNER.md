# Site QCXZ : images et vidéos à faire

Mets chaque image dans `assets/shots/` avec **exactement** le nom indiqué (JPG, 1920x1080). Tant qu'une image
manque, le site affiche une carte qui décrit le plan. Dès que le fichier existe, la photo apparaît toute seule.

## Conseils

- Cache le HUD, graphismes au max, distance de vue haute.
- Coucher de soleil ou nuit avec lumières : le jeu est bien plus beau qu'à midi.
- Fais jouer 3-6 amis comme figurants : un serveur vide en photo, ça fait fuir.
- Des couleurs qui rappellent le logo aident (gyrophares bleus, néons, ciel violet au crépuscule).

## Screenshots (5)

| Fichier | Ce qu'on doit voir |
|---|---|
| `01-hero.jpg` | Grande image en tête de galerie et aperçu de la vidéo. Coucher de soleil : joueurs et chars devant le poste de police de Saint-Philippe, gyrophares allumés. Prends ton temps sur celle-là. |
| `02-police.jpg` | Arrestation de nuit, éclairée par les gyrophares rouge et bleu. |
| `03-cars.jpg` | 5-6 chars variés alignés : pick-up surélevé, sportive, voiture de police, moto. |
| `04-gang.jpg` | Un groupe d'amis posé devant ses véhicules dans un coin isolé. |
| `05-work.jpg` | Un joueur qui récolte à la carrière, à la mine ou au verger. |

## Vidéos

### Bande-annonce : `assets/video/trailer.mp4` (45-60 s, 1080p, MP4 H.264, moins de 40 Mo)

Trop lourde pour ton hébergement ? Mets-la sur YouTube et colle le lien dans `YOUTUBE_URL` en bas de `index.html`.

1. **0-5 s** : vue aérienne qui descend sur Saint-Philippe au lever du soleil. Le logo QCXZ apparaît.
2. **5-15 s** : la vie normale : récolte, camion vers la raffinerie, achat d'un char.
3. **15-25 s** : la nuit tombe, un deal, une voiture de police ralentit.
4. **25-40 s** : poursuite, sirènes, arrestation.
5. **40-50 s** : la bande d'amis qui roule en convoi, rires, ville éclairée.
6. **50-60 s** : logo + « Serveurs communautaires › QCXZ » + Discord.

### Clips courts (vertical 9:16, 15-30 s, pour TikTok / Reels / Shorts)

- « Ma première journée à 0 $ »
- « La police d'Everon ne niaise pas »
- « Le cell qui fait tout »

### Outils

- OBS Studio (gratuit) en 1080p60, ou NVIDIA ShadowPlay pour garder les 30 dernières secondes d'un moment drôle.
- Montage : DaVinci Resolve (gratuit) ou CapCut pour le vertical.

## Avant de mettre en ligne

En bas de `index.html` :

```js
const DISCORD_URL = "";   // ton lien d'invitation Discord
const YOUTUBE_URL = "";   // optionnel : la bande-annonce
```

Mets `index.html` et le dossier `assets/` (le logo est déjà dedans) sur un hébergeur statique : Cloudflare Pages,
GitHub Pages ou Netlify.
