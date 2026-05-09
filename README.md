# NetFloow

Thème CSS style Netflix pour Jellyfin 10.11.x.

![Version](https://img.shields.io/badge/version-1.0.0-E50914?style=flat-square)
![Jellyfin](https://img.shields.io/badge/Jellyfin-10.11.x-00A4DC?style=flat-square)

---

## Installation

Dans Jellyfin : **Tableau de bord → Général → Slogan → Code CSS personnalisé**

```css
/* Production — branche main */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@main/netfloow.css");
```

```css
/* Test — hash de commit (recommandé) */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@COMMIT_HASH/netfloow.css");
```

---

## Variantes

```css
/* Fond noir pur — écrans OLED */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@main/variants/netfloow-oled.css");

/* Thème bleu */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@main/variants/netfloow-blue.css");
```

---

## Addons

```css
/* Scrollers horizontaux améliorés */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@main/addons/scrollers.css");

/* Overrides plugin Media Bar (IAmParadox) */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@main/addons/mediabar.css");

/* Page de connexion personnalisée */
@import url("https://cdn.jsdelivr.net/gh/DeiLucri/NetFloow@main/addons/login.css");
```

---

## Structure

```
NetFloow/
  netfloow.css              → thème principal (15 sections)
  variants/
    netfloow-oled.css       → fond noir pur OLED
    netfloow-blue.css       → variante bleue
  addons/
    scrollers.css           → scrollers horizontaux homepage
    mediabar.css            → overrides plugin Media Bar
    login.css               → page connexion custom
  assets/
    logo.svg                → logo NetFloow vectoriel
  README.md
  CHANGELOG.md
```

---

## Configuration

Toutes les valeurs sont dans le bloc `:root` en tête de `netfloow.css`. Aucune valeur n'est hardcodée.

| Variable | Valeur | Description |
|---|---|---|
| `--nf-primary` | `229, 9, 20` | Rouge principal (#E50914) |
| `--nf-bg` | `10, 10, 10` | Background (#0A0A0A) |
| `--nf-font-primary` | Outfit | Police UI |
| `--nf-font-logo` | Bebas Neue | Police logo |
| `--nf-hover-scale` | `1.05` | Zoom hover cartes |
| `--nf-transition` | `0.3s` | Vitesse animations |

---

## Compatibilité

| Client | Support |
|---|---|
| Navigateurs (Chrome, Firefox) | ✅ |
| Jellyfin Desktop 2.0.0+ | ✅ |
| App Android mobile | ✅ |
| Android TV | ⚠️ partiel |
| Apps TV natives (Apple TV, Roku) | ❌ |

---

## Plugins supportés

- Home Screen Sections (IAmParadox)
- Media Bar (IAmParadox)
- Jellyfin Enhanced (n00bcodr)
- KefinTweaks (ranaldsgift)
- Intro Skipper

---

## Référence

- [Doc CSS Jellyfin officielle](https://jellyfin.org/docs/general/clients/css-customization)
- [Finimalism](https://github.com/tedhinklater/finimalism) — référence d'architecture
