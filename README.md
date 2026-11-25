# 💌 Dawat Digital

Shadi, mehndi, walima, birthday aur aqeeqah ke liye **premium digital invitations** ki website.
Chhape hue card ki jagah ek link jo music, countdown, Google Maps aur RSVP ke saath khulta hai.

Ye ek single-file website hai (`index.html`), is liye GitHub Pages par bina kisi build ya install ke chalti hai.

---

## ✨ Website mein kya hai

| Hissa | Tafseel |
|---|---|
| **Home** | Envelope opening animation, live countdown, features, chhape card se mukabla, packages, process aur FAQ |
| **Catalog** | 16 ready-made designs, Shadi / Mehndi / Birthday / Aqeeqah ke filter, har design par WhatsApp "Order" button |
| **Packages** | Basic (PKR 1,500), Premium (PKR 3,500), Royal (PKR 7,500) |
| **Live Demo** | Har package ka alag demo, jis mein farq saaf nazar aata hai (Basic, Premium, Royal) |
| **WhatsApp** | Har button par message pehle se likha hua aata hai (package ya design ka naam ke saath) |

### Teen packages ka farq

| Feature | Basic | Premium | Royal |
|---|:---:|:---:|:---:|
| Animated invitation | ✅ | ✅ | ✅ |
| Google Maps link | ✅ | ✅ | ✅ |
| Music | ❌ | ✅ | ✅ |
| Live countdown | ❌ | ✅ | ✅ |
| RSVP form | ❌ | ✅ | ✅ |
| Photo gallery | ❌ | 10 tak | Unlimited |
| Print-ready PDF | ❌ | ✅ | ✅ |
| Mehndi / Barat / Walima ke alag pages | ❌ | ❌ | ✅ |
| 100% custom design | ❌ | ❌ | ✅ |
| Apna domain (naam.com) | ❌ | ❌ | ✅ |
| Link ki muddat | 30 din | 1 saal | 1 saal |

---

## 🚀 GitHub Pages par host karne ka tareeqa

1. GitHub par naya repository banayein (misal: `dawat-digital`).
2. Is repository mein `index.html` aur `README.md` upload karein.
3. **Settings → Pages** kholein.
4. **Source** mein `Deploy from a branch` chunein.
5. **Branch** `main` aur folder `/ (root)` select karke **Save** dabayein.
6. 1 se 2 minute baad website yahan live hogi:
   `https://USERNAME.github.io/dawat-digital/`

> Apna domain lagana ho to Pages settings mein **Custom domain** mein domain likh dein.

---

## 🛠️ Apni details badalna

Sab kuch `index.html` ke andar `<script>` mein hai. Sab se upar **SETTINGS** ka hissa dekhein:

```js
var PHONE="923170114485";             // WhatsApp number (92 se shuru, bina + ya 0 ke)
var EVENT_DATE="2027-02-14T19:00:00"; // hero aur demo ki countdown date
```

### Qeematein aur package ki details

`PLANS` list mein har package ka `price`, `sub` (tareef), `ok` (jo milta hai) aur `no` (jo nahi milta) badal sakte hain.

```js
{id:"premium", name:"Premium", price:3500, sub:"...", ok:[...], no:[]}
```

### Naya template catalog mein jodna

`TPL` list mein ek nayi line add karein:

```js
["Design ka naam", "Category", "package", "rang1,rang2", "emoji", "Naam", "Taqreeb ka title"]
```

Misal:

```js
["Neelam Nikah","Shadi","premium","#0b2a5b,#5b8def","💎","Omar & Laiba","Nikah Ki Dawat"]
```

- **Category:** `Shadi`, `Mehndi`, `Birthday` ya `Aqeeqah`
- **package:** `basic`, `premium` ya `royal` (qeemat khud package se aati hai)
- **Rang:** card ke gradient ke do rang (hex code)

Naya category chahiye to `CATS` list mein bhi uska naam add kar dein.

---

## 📁 Files

```
dawat-digital/
├── index.html   # poori website (home, catalog, demos)
└── README.md    # ye file
```

## 🔗 Pages ke links

| Page | Link |
|---|---|
| Home | `/` |
| Catalog | `/#catalog` |
| Basic demo | `/#demo-basic` |
| Premium demo | `/#demo-premium` |
| Royal demo | `/#demo-royal` |

Ye links WhatsApp, Instagram bio ya reels mein seedha share kiye ja sakte hain.

---

## 📝 Zaroori baatein

- Demo mein music ek simple browser-generated dhun hai. Asli orders mein customer ka pasandida gana lagayein.
- Demo ka RSVP sirf screen par dikhta hai, kahin save nahi hota. Asli orders ke liye Google Form ya Google Sheet jod sakte hain.
- Website mein fonts Google Fonts se aate hain, is liye internet zaroori hai.
- Design phone ke liye bhi theek chalta hai, lekin publish karne se pehle apne phone par ek dafa zaroor check karein.

## 📞 Rabta

WhatsApp par order dein: **0317 0114485**
