# Nikunj Rathva — Portfolio Website (README)

આ file માં તમારી website ને **edit કરવાની**, **mobile પર જોવાની**, અને **free માં live/publish કરવાની** સંપૂર્ણ સ્ટેપ-બાય-સ્ટેપ માહિતી છે. સરળ ભાષામાં લખેલું છે, coding ની જરૂર નથી.

---

## 1. Files સમજો

```
nikunj-portfolio/
├── index.html      → Website નું content (text, sections)
├── css/style.css   → Website નો look (colors, design, layout)
├── js/script.js    → Menu, form, animations નું logic
└── README.md       → આ file
```

Content બદલવા માટે ફક્ત **index.html** ખોલો — બાકીની files ને હાથ લગાડવાની જરૂર નથી.

---

## 2. તમારી માહિતી ભરો (Placeholders)

`index.html` ખોલો અને `[ ]` bracket માં લખેલી બધી જગ્યાઓ શોધો (Ctrl+F / mobile માં "Find" વાપરીને `[` search કરો) અને તમારી real details થી replace કરો:

| Placeholder | શું ભરવું |
|---|---|
| `[YOUR BIO]` | તમારા વિશે 2-4 lines |
| `[YOUR PHOTO]` | તમારો ફોટો (નીચે સ્ટેપ 3 જુઓ) |
| `[YOUR WHATSAPP]` | 10-digit number, દા.ત. `9876543210` |
| `[YOUR EMAIL]` | તમારો email (2 જગ્યાએ છે: HTML અને script.js બંનેમાં) |
| `[YOUR LINKEDIN LINK]` / `[YOUR GITHUB LINK]` / `[YOUR INSTAGRAM LINK]` | તમારી profile links |
| `[PROJECT NAME 1/2/3]`, `[PROJECT IMAGE]` | તમારા projects ની details |
| `[YOUR TARGET DATE]` | તમારો goal date |

**Tip:** Mobile browser (Chrome) માં કોઈપણ `.html` file ને "Text Editor" app (દા.ત. **Acode**, **Quoted**, કે **Text Editor - Notepad**) થી ખોલીને edit કરી શકાય છે — coding knowledge વગર પણ, ફક્ત text બદલવાનું છે.

---

## 3. તમારો ફોટો ઉમેરવો

1. `images` નામનું folder છે — તમારો ફોટો ત્યાં mukો (દા.ત. `myphoto.jpg`).
2. `index.html` માં આ line શોધો:
   ```html
   <div class="hero__photo">[YOUR PHOTO]</div>
   ```
3. તેને આ પ્રમાણે બદલો:
   ```html
   <div class="hero__photo"><img src="images/myphoto.jpg" alt="Nikunj Rathva"></div>
   ```

Project images માટે પણ એ જ રીતે `.project-card__image` વાળી div ને `<img>` tag થી replace કરી શકાય.

---

## 4. Mobile પરથી Website કેવી રીતે "Run" કરીને જોવી

તમારે coding software ની જરૂર નથી, ફક્ત browser જોઈએ:

1. Files ને તમારા phone ના **Files app** માં એક folder માં save કરો (જેમ કે `nikunj-portfolio`).
2. `index.html` file પર tap કરો → "Open with" માં **Chrome** (કે કોઈપણ browser) select કરો.
3. તમારી website ત્યાં જ ખૂલી જશે — બધું check કરો (scroll, buttons, mobile menu).
4. Edit કરવા માટે → same file ને "Acode" કે "Text Editor" app થી ખોલો, બદલો, save કરો, અને Chrome માં refresh કરો.

---

## 5. Website ને FREE માં Internet પર Publish કરવી

નીચે 2 સહેલા free options છે — બંને માટે કોઈ paid service જરૂરી નથી.

### Option A: GitHub Pages (સૌથી popular, free forever)

1. Mobile browser માં [github.com](https://github.com) પર જાઓ અને free account બનાવો.
2. "+" icon → **New repository** → નામ આપો, દા.ત. `nikunj-portfolio` → **Public** રાખો → Create.
3. Repository ખૂલશે ત્યાં **"uploading an existing file"** link પર tap કરો.
4. તમારી બધી files (index.html, css folder, js folder) upload કરો (folder structure સાચવીને).
5. **Commit changes** કરો.
6. Repository ના **Settings** → ડાબી બાજુ **Pages** → Source માં "main" branch select કરી **Save** કરો.
7. થોડી મિનિટોમાં તમને એક link મળશે: `https://yourusername.github.io/nikunj-portfolio/` — આ તમારી live website છે! આ link WhatsApp, resume, business card બધે share કરી શકાય.

### Option B: Netlify Drop (સૌથી ઝડપી, drag-and-drop)

1. Browser માં [app.netlify.com/drop](https://app.netlify.com/drop) ખોલો.
2. તમારો `nikunj-portfolio` folder (zip કરીને અથવા files select કરીને) drag-drop કરો.
3. થોડી સેકંડમાં website live થઈ જશે અને એક free link મળશે (દા.ત. `random-name.netlify.app`).
4. Free account બનાવીને પછી custom name પણ set કરી શકાય.

---

## 6. Contact Form વિશે સમજ

Form submit થાય ત્યારે તે તમારા **email app ને ખોલશે** (Gmail/Outlook) અને message ready-made ભરેલો હશે — user એ ફક્ત "Send" દબાવવાનું રહેશે. આ maટે કોઈ backend/paid service જોઈતી નથી.

**Advanced (optional):** જો તમારે form directly submit થાય (email app ખોલ્યા વગર) એવું જોઈતું હોય, તો free service **Formspree.io** પર account બનાવીને, form ના `action` attribute માં તેમનું endpoint URL ઉમેરી શકાય. હાલ માટે mailto method simple અને free છે.

---

## 7. આગળ શું કરવું

- WhatsApp number અને email confirm કરો કે બરાબર કામ કરે છે.
- 2-3 real projects ઉમેરો (screenshots લઈને `images` folder માં મૂકો).
- Website live થાય પછી link ને WhatsApp status, Instagram bio, resume માં add કરો.
- Comfortable થાવ પછી CSS colors (`css/style.css` ના ઉપરના ભાગમાં `:root` variables) બદલીને પોતાનો style પણ try કરી શકો છો.

Good luck, Nikunj! 🚀
