# Analyse de sols du Québec (2007-2024)

Tableaux de bord interactifs présentant l'évolution spatio-temporelle d'indicateurs de chimie-fertilité, basés sur les analyses de plus de 600 000 échantillons de sols agricoles du Québec.
## Aperçu

Ce tableau de bord permet de visualiser et de comparer les données d'analyses de sols à l'échelle des régions administratives et des MRC du Québec, de 2007 à 2024. Les données provenant de deux laboratoires privés ont été acquises au cours du temps par le MAPAQ et sont présentées ici dans le cadre du mécanisme mis en oeuvre pour suivre l'état de santé des sols agricoles du Québec.

### Indicateurs présentés

- **P, K, Ca, Mg** - Phosphore, potassium, calcium, magnésium extraits en solution Mehlich-3 et exprimés en kg/ha
- **Al, Fe, Mn, Cu** - Aluminium, fer, manganèse, cuivre extraits en solution Mehlich-3 et exprimés en ppm ou mg/kg 

- **pH eau** - pH mesuré dans un ratio sol-eau de 1:1; exprime le niveau d'acidité du sol
- **pH tampon** - pH mesuré en solution SMP; exprime la réserve d'acidité du sol
- **Besoin en chaux (t/ha)**  - Amendement calcique recommandé pour un IVA (Indice de Valeur Alcalinisante) de 100 %

- **Matière organique (%)**  - Teneur en matière organique du sol
- **Analyses >= 4% MO (%)**  - Pourcentage d'échantillons de sol avec plus de 4 % de MO, le seuil ciblé dans le Plan d'agriculture durable

- **ISP - G1** (%) - Indice de saturation en phosphore et risque environnemental dans les sols lourds (groupe textural G1)
- **ISP - G2-G3** (%) - Indice de saturation en phosphore et risque environnemental dans les sols moyens et légers (groupes texturaux G2 et G3)
- **CEC (méq/100g)**  - Capacité d'échange cationique calculée avec la somme des bases et le pH tampon

### Fonctionnalités

- Visualisation cartographique interactive (MapLibre GL + PMTiles)
- Deux échelles géographiques (Région / Municipalité régionale de comté (MRC))
- Choix de la statistique (Médiane / Moyenne)
- Filtrage par année ou vue globale
- Tableau de données triable et filtrable
- Exportation des données en fichiers CSV
- Interface réactive (mobile/tablette/desktop)

## Technologies

- **Cartographie** : [MapLibre GL JS](https://maplibre.org/) + [PMTiles](https://protomaps.com/docs/pmtiles)
- **Fond de carte** : Carte du gouvernement du Québec
- **Données** : JSON optimisé (~1 Mo)
- **Hébergement** : GitHub Pages (statique, sans serveur)

## Fichiers

| Fichier | Description |
|---------|-------------|
| `index.html` | Application complète (HTML/CSS/JS) |
| `data.json` | Données agrégées par région/MRC et année |
| `mrc.pmtiles` | Tuiles vectorielles des MRC |
| `region.pmtiles` | Tuiles vectorielles des régions |

## Source des données

Les données proviennent d'analyses d'échantillons de sols acquises par le MAPAQ auprès de deux laboratoires privés entre 2007 et 2024. Elles ont été filtrées, nettoyées, géolocalisées, et agrégées par l'IRDA.

### Limites d'interprétation

- La géolocalisation repose sur les codes postaux (incertitude spatiale variable)
- Les protocoles d'échantillonnage des sols ne sont pas aléatoires ni systématiques
- Certains échantillons peuvent provenir de milieux non agricoles

## Contact

- **Cédric Bouffard**, professionnel de recherche : cedric.bouffard@irda.qc.ca
- **Marc-Olivier Gasser**, chercheur : marc-o.gasser@irda.qc.ca

## Partenaires

<p align="center">
  <a href="https://www.quebec.ca/">
    <img src="https://www.foretouverte.gouv.qc.ca/particular/images/QUEB.png" alt="Gouvernement du Québec" height="50">
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.irda.qc.ca/">
    <img src="https://irda.qc.ca/dist/assets/logos/logo-irda-color.svg" alt="IRDA" height="40">
  </a>
</p>

## Licence

Ce projet est sous licence [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) (Attribution - Pas d'utilisation commerciale).

© IRDA - Institut de recherche et de développement en agroenvironnement
