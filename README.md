# Pharmacie Foufou Ali — Charte Graphique E-Commerce

Projet : Site e-commerce parapharmacie & cosmétiques  
Client : Pharmacie Foufou Ali  
Site vitrine existant : [pharmacie-foufouali.com](https://pharmacie-foufouali.com)  
Référence stylistique : pharmaly-dz.com  

---

## 1. Palette de Couleurs

### Couleurs Primaires & Nuances de Vert

| Rôle | Nom | Hex | Usage |
|------|-----|-----|-------|
| Vert très foncé | `--color-green-900` | `#064A2A` | Textes forts sur fond clair, footer |
| Vert foncé | `--color-green-700` | `#08A05A` | Hover boutons, titres |
| Vert principal (marque) | `--color-primary` | `#0BC270` | CTA, boutons, icônes actives |
| Vert moyen | `--color-green-400` | `#0DD980` | Accents secondaires |
| Vert doux | `--color-green-200` | `#5EE8AA` | Éléments décoratifs, illustrations |
| Vert pâle | `--color-green-100` | `#A8F2D1` | Badges, chips catégories |
| Vert très clair | `--color-green-50` | `#E8FBF3` | Fonds de sections alternées |
| Vert ultra pâle | `--color-green-25` | `#F0FDF8` | Fonds de cartes, hover léger |

### Couleurs Neutres

| Rôle | Nom | Hex | Usage |
|------|-----|-----|-------|
| Blanc pur | `--color-white` | `#FFFFFF` | Fond pages, cartes produits |
| Gris très clair | `--color-gray-50` | `#F8F9FA` | Fond sections alternées |
| Gris clair | `--color-gray-100` | `#F1F3F5` | Bordures, séparateurs |
| Gris moyen | `--color-gray-400` | `#ADB5BD` | Texte secondaire, placeholders |
| Gris texte | `--color-gray-600` | `#6C757D` | Descriptions produits |
| Texte principal | `--color-text` | `#1A1A2E` | Corps de texte, titres |

### Couleurs Fonctionnelles

| Rôle | Nom | Hex | Usage |
|------|-----|-----|-------|
| Succès | `--color-success` | `#0BC270` | Confirmations, "En stock" |
| Erreur | `--color-error` | `#E63946` | Erreurs, "Rupture de stock" |
| Avertissement | `--color-warning` | `#FF9F1C` | Promotions, "Derniers articles" |
| Info | `--color-info` | `#2196F3` | Notifications informatives |

### Couleurs Cosmétiques (Accents Spéciaux)

Ces teintes servent à différencier les catégories sur le site :

| Catégorie | Hex | Usage |
|-----------|-----|-------|
| Soins visage | `#F4A7B9` | Badge / filtre catégorie |
| Cheveux | `#C8A97E` | Badge / filtre catégorie |
| Corps & bien-être | `#A8DADC` | Badge / filtre catégorie |
| Hygiène | `#90E0EF` | Badge / filtre catégorie |
| Bébé | `#FFD6E0` | Badge / filtre catégorie |

---

## 2. Typographie

### Polices Principales

```
Titres      → Poppins (Google Fonts)
Corps       → Roboto (Google Fonts)
UI / Prix   → Inter (Google Fonts)
```

> Ces trois polices sont gratuites, disponibles sur Google Fonts, et très bien adaptées au e-commerce moderne.

### Import Google Fonts

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&family=Roboto:wght@300;400;500&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

### Échelle Typographique

| Élément | Police | Taille | Poids | Couleur |
|---------|--------|--------|-------|---------|
| H1 (Hero / page title) | Poppins | 40–48px | 700–800 | `#0C2460` |
| H2 (Section title) | Poppins | 28–32px | 700 | `#0C2460` |
| H3 (Titre produit / carte) | Poppins | 18–22px | 600 | `#1A1A2E` |
| H4 (Sous-section) | Poppins | 16–18px | 600 | `#1A1A2E` |
| Corps de texte | Roboto | 15–16px | 400 | `#1A1A2E` |
| Texte secondaire | Roboto | 13–14px | 400 | `#6C757D` |
| Prix principal | Inter | 20–24px | 700 | `#0BC270` |
| Prix barré | Inter | 15px | 400 | `#ADB5BD` |
| Bouton CTA | Poppins | 14–16px | 600 | `#FFFFFF` |
| Label / Badge | Inter | 11–12px | 600 | Variable |
| Navigation | Roboto | 15px | 500 | `#0C2460` |

### Variables CSS Typographiques

```css
:root {
  --font-heading: 'Poppins', sans-serif;
  --font-body: 'Roboto', sans-serif;
  --font-ui: 'Inter', sans-serif;

  --text-xs:   0.75rem;   /* 12px */
  --text-sm:   0.875rem;  /* 14px */
  --text-base: 1rem;      /* 16px */
  --text-lg:   1.125rem;  /* 18px */
  --text-xl:   1.25rem;   /* 20px */
  --text-2xl:  1.5rem;    /* 24px */
  --text-3xl:  1.875rem;  /* 30px */
  --text-4xl:  2.25rem;   /* 36px */
  --text-5xl:  3rem;      /* 48px */

  --font-light:    300;
  --font-regular:  400;
  --font-medium:   500;
  --font-semibold: 600;
  --font-bold:     700;
  --font-extrabold:800;

  --leading-tight:  1.25;
  --leading-normal: 1.5;
  --leading-relaxed:1.625;
}
```

---

## 3. Variables CSS Complètes (Design Tokens)

```css
:root {
  /* === COULEURS === */
  --color-green-900:  #064A2A;
  --color-green-700:  #08A05A;
  --color-primary:    #0BC270;
  --color-green-400:  #0DD980;
  --color-green-200:  #5EE8AA;
  --color-green-100:  #A8F2D1;
  --color-green-50:   #E8FBF3;
  --color-green-25:   #F0FDF8;

  --color-white:     #FFFFFF;
  --color-gray-50:   #F8F9FA;
  --color-gray-100:  #F1F3F5;
  --color-gray-400:  #ADB5BD;
  --color-gray-600:  #6C757D;
  --color-text:      #1A1A2E;

  --color-success:   #0BC270;
  --color-error:     #E63946;
  --color-warning:   #FF9F1C;
  --color-info:      #2196F3;

  /* === TYPOGRAPHIE === */
  --font-heading:    'Poppins', sans-serif;
  --font-body:       'Roboto', sans-serif;
  --font-ui:         'Inter', sans-serif;

  /* === ESPACEMENTS === */
  --space-xs:   0.25rem;   /*  4px */
  --space-sm:   0.5rem;    /*  8px */
  --space-md:   1rem;      /* 16px */
  --space-lg:   1.5rem;    /* 24px */
  --space-xl:   2rem;      /* 32px */
  --space-2xl:  3rem;      /* 48px */
  --space-3xl:  4rem;      /* 64px */

  /* === BORDER RADIUS === */
  --radius-sm:  4px;
  --radius-md:  8px;
  --radius-lg:  12px;
  --radius-xl:  16px;
  --radius-full:9999px;

  /* === OMBRES === */
  --shadow-sm:  0 1px 3px rgba(0,0,0,0.08);
  --shadow-md:  0 4px 12px rgba(0,0,0,0.10);
  --shadow-lg:  0 8px 24px rgba(0,0,0,0.12);
  --shadow-card:0 2px 8px rgba(12,36,96,0.08);

  /* === TRANSITIONS === */
  --transition-fast:   150ms ease;
  --transition-normal: 250ms ease;
  --transition-slow:   400ms ease;
}
```

---

## 4. Composants Visuels Clés

### Boutons

| Type | Fond | Texte | Bordure |
|------|------|-------|---------|
| Primaire (Ajouter au panier) | `#0BC270` | `#FFFFFF` | — |
| Secondaire (Voir détails) | `transparent` | `#064A2A` | `1px solid #0BC270` |
| Danger (Supprimer) | `#E63946` | `#FFFFFF` | — |
| Ghost (secondaire léger) | `#E8FBF3` | `#08A05A` | — |

### Cartes Produit

- Fond : `#FFFFFF`
- Ombre : `--shadow-card`
- Border-radius : `--radius-lg` (12px)
- Badge promo : fond `#FF9F1C`, texte blanc, `--radius-full`
- Badge "Nouveau" : fond `#0BC270`, texte blanc
- Badge "Rupture" : fond `#ADB5BD`, texte blanc

---

## 5. Références & Inspirations

| Ressource | Lien |
|-----------|------|
| Site vitrine client | https://pharmacie-foufouali.com |
| Instagram | https://www.instagram.com/ali.adem.5492216/ |
| Facebook | https://www.facebook.com/profile.php?id=100063508722874 |
| LinkedIn | https://www.linkedin.com/in/ali-foufou-alg%C3%A9rie-3191a691/ |
| Site référence style | pharmaly-dz.com |

---

## 6. Principes de Design

- **Clarté avant tout** : fond blanc dominant, air et espace entre les éléments
- **Confiance médicale** : bleu marine pour les éléments institutionnels (header, footer, titres)
- **Dynamisme santé** : vert vif pour les CTA et éléments interactifs
- **Hiérarchie visuelle** : prix toujours en vert et gras, noms produits en Poppins semibold
- **Mobile-first** : conçu d'abord pour les smartphones (majorité du trafic DZ)
- **Accessibilité** : contraste WCAG AA minimum sur tous les textes

---

*Document créé le 2026-04-12 — à mettre à jour au fil des itérations client.*
