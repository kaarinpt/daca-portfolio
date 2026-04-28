# 🚀 Meeskonna Portfoolio

> Kõik lingid, ligipääsud ja seadistused ühes kohas.

---

## 📋 Sisukord

- [Repositooriumi info](#repositooriumi-info)
- [Meeskond ja ligipääsud](#meeskond-ja-ligipääsud)
- [Kataloogistruktuur](#kataloogistruktuur)
- [Seadistus – alustamine](#seadistus--alustamine)
- [Olulised lingid](#olulised-lingid)
- [Keskkonna muutujad](#keskkonna-muutujad)

---

## 📦 Repositooriumi info

| Väli | Info |
|------|------|
| **Repositoorium** | `https://github.com/ORGANISATSIOON/portfoolio` |
| **Peaharu** | `main` |
| **Litsents** | MIT |
| **Loodud** | 2026 |

---

## 👥 Meeskond ja ligipääsud

| Nimi | Roll | GitHub kasutajanimi | Ligipääsutase |
|------|------|----------------------|---------------|
| Nimi Perenimi | Tech Lead | @kasutajanimi | Admin |
| Nimi Perenimi | Frontend | @kasutajanimi | Write |
| Nimi Perenimi | Backend | @kasutajanimi | Write |
| Nimi Perenimi | Designer | @kasutajanimi | Read |

### Ligipääsu lisamine
1. Mine **GitHub → repositoorium → Settings → Collaborators**
2. Klõpsa „Add people"
3. Otsi kasutajanime järgi ja vali roll

---

## 📁 Kataloogistruktuur

```
portfoolio/
├── README.md                  # See fail – seadistused ja lingid
├── .gitignore                 # Ignoreeritavad failid
├── .env.example               # Keskkonna muutujate näidis
│
├── docs/                      # Dokumentatsioon
│   ├── setup.md               # Detailne seadistusjuhend
│   ├── contributing.md        # Panustamise juhend
│   └── api.md                 # API dokumentatsioon
│
├── src/                       # Lähtekood
│   ├── components/            # Korduvkasutatavad komponendid
│   ├── pages/                 # Leheküljed
│   ├── assets/                # Pildid, fondid, ikoonid
│   └── styles/                # CSS / SCSS failid
│
├── projects/                  # Meeskonna projektid
│   ├── projekt-1/
│   ├── projekt-2/
│   └── projekt-3/
│
├── members/                   # Liikmete profiilid
│   ├── liige-1.md
│   └── liige-2.md
│
└── public/                    # Staatilised failid (build väljund)
```

---

## ⚙️ Seadistus – alustamine

### 1. Klooni repositoorium
```bash
git clone https://github.com/ORGANISATSIOON/portfoolio.git
cd portfoolio
```

### 2. Installi sõltuvused
```bash
npm install
```

### 3. Seadista keskkonna muutujad
```bash
cp .env.example .env
# Ava .env ja täida väärtused
```

### 4. Käivita arendusserver
```bash
npm run dev
```

---

## 🔗 Olulised lingid

### GitHub
| Link | Kirjeldus |
|------|-----------|
| [Repositoorium](https://github.com/ORGANISATSIOON/portfoolio) | Peamise koodi asukoht |
| [Issues](https://github.com/ORGANISATSIOON/portfoolio/issues) | Vigade ja ülesannete jälgimine |
| [Pull Requests](https://github.com/ORGANISATSIOON/portfoolio/pulls) | Koodiülevaatused |
| [Actions](https://github.com/ORGANISATSIOON/portfoolio/actions) | CI/CD pipelines |
| [Settings](https://github.com/ORGANISATSIOON/portfoolio/settings) | Repositooriumi seaded |

### Meeskonnatöö tööriistad
| Tööriist | Link | Eesmärk |
|----------|------|---------|
| Figma | https://figma.com/... | Disainifailid |
| Notion | https://notion.so/... | Dokumentatsioon |
| Slack | https://meeskond.slack.com | Suhtlus |
| Vercel / Netlify | https://... | Deploy ja hosting |

### Elav sait
| Keskkond | URL | Haru |
|----------|-----|------|
| Production | https://portfoolio.ee | `main` |
| Staging | https://staging.portfoolio.ee | `staging` |
| Development | http://localhost:3000 | lokaalne |

---

## 🔐 Keskkonna muutujad

Loo `.env` fail projekti juurkausta (ära kunagi lisa Giti!):

```env
# Üldised
VITE_APP_NAME=Meeskonna Portfoolio
VITE_APP_URL=https://portfoolio.ee

# API
VITE_API_URL=https://api.portfoolio.ee
VITE_API_KEY=sinu_api_võti_siia

# Andmebaas (ainult backend)
DATABASE_URL=postgresql://kasutaja:parool@localhost:5432/portfoolio
```

> ⚠️ `.env` on lisatud `.gitignore` faili – ära kunagi lae päris võtmeid GitHubi!

---

## 🌿 Harustrateegia (Branching)

```
main          ← stabiilne, production
staging       ← testimine enne toodangut
feature/...   ← uued funktsioonid (nt feature/avaleht)
fix/...       ← veaparandused (nt fix/navigatsioon)
```

### Tüüpiline töövoog
```bash
git checkout -b feature/minu-funktsioon
# tee muudatused
git add .
git commit -m "Lisa: uus funktsioon"
git push origin feature/minu-funktsioon
# Ava Pull Request GitHubis
```

---

## 📞 Kontakt ja abi

Küsimuste korral:
- **GitHub Issues** – tehniline abi
- **Slack #portfoolio** – kiired küsimused
- **Tech Lead:** nimi@email.ee

---

*Viimati uuendatud: Aprill 2026*
