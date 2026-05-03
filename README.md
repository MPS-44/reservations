# 📋 Guide — Remplir les tarifs dans les formulaires

## Les fichiers à modifier

| Fichier | Appareil | Tarifs à remplacer |
|---|---|---|
| aspirateur-hkoenig.html | Aspirateur HKoenig UMAT40 | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| aspirateur-karcher-vch4.html | Kärcher VCH4 ✅ déjà rempli | 9€ / ? / 14€ / 22€ / 39€ — caution 119€ (remplacer TARIF_2J si besoin) |
| beer-up.html | Tireuse Beer-UP | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| bissell-spotclean.html | Bissell ✅ déjà rempli | 19/25/29/49/79€ — caution 219€ |
| karcher-sc1.html | Nettoyeur vapeur SC1 | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| karcher-k3.html | Haute pression K3 | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| lave-vitres-puruikai.html | Robot Puruikai | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| machine-a-glace.html | Machine à glace ✅ déjà rempli | 3 formules complètes |
| ordinateur-dell.html | Dell Inspiron | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| ordinateur-hp17.html | HP 17 pouces | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| robot-abir-wd8.html | Robot Abir WD8 | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| robot-ecovacs-winbot.html | Robot Ecovacs Winbot | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| samsung-galaxy-s10.html | Samsung Galaxy S10 | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |
| thomson-thmsc1500.html | Injecteur Thomson | TARIF_1J / TARIF_2J / TARIF_WE / TARIF_SEM / TARIF_MOIS + TARIF_CAUTION_€ |

## Comment modifier un fichier

1. Ouvre le fichier dans un éditeur de texte (Notepad, VS Code...)
2. Utilise **Ctrl+H** (Rechercher/Remplacer)
3. Remplace chaque placeholder par le vrai tarif :
   - `TARIF_1J` → ex: `9`
   - `TARIF_2J` → ex: `14`
   - `TARIF_WE` → ex: `19`
   - `TARIF_SEM` → ex: `35`
   - `TARIF_MOIS` → ex: `59`
   - `TARIF_CAUTION_€` → ex: `119 €`

## Mettre en ligne sur GitHub Pages

1. Va sur github.com → connecte-toi avec MPS-44
2. Crée un nouveau repository : **reservations**
3. Uploade tous les fichiers HTML (bouton "Add file → Upload files")
4. Va dans Settings → Pages → Source: **main** → Save
5. Tes formulaires seront accessibles sur :
   `https://mps-44.github.io/reservations/bissell-spotclean.html`
   `https://mps-44.github.io/reservations/machine-a-glace.html`
   etc.

## Intégrer en iframe dans Odoo

Dans chaque page formulaire Odoo, ajoute un bloc "Embed Code" et colle :

```html
<iframe 
  src="https://mps-44.github.io/reservations/NOMFICHIER.html" 
  width="100%" 
  height="1100" 
  frameborder="0" 
  style="border:none;border-radius:12px;">
</iframe>
```

Remplace `NOMFICHIER` par le nom du fichier correspondant.
