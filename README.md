# sewhail

ultra-minimal portfolio website with a nerdy, terminal-inspired aesthetic.

## stack

- **next.js 16** - react framework
- **typescript** - type safety
- **tailwind css 4** - styling
- **shadcn/ui** - component library
- **lucide-react** - icons
- **jetbrains mono** - monospace font

## features

- 🌓 light/dark mode toggle
- 💻 terminal-style design (`$ whoami`, `>` prefixes)
- 🔤 monospace typography (jetbrains mono, fira code)
- 📱 fully responsive
- ⚡ ultra-minimal aesthetic (9-10px fonts, no rounded corners)
- 🔗 working social links (github, twitter, linkedin)
- 📧 clickable email
- 🎨 custom favicon

## local development

```bash
# install dependencies
npm install

# run dev server
npm run dev
```

open [http://localhost:3000](http://localhost:3000)

## deployment

### cloudflare pages (recommended)

1. push to github
2. go to [cloudflare pages](https://pages.cloudflare.com)
3. connect github repo
4. configure build:
   - **framework**: next.js
   - **build command**: `npm run build`
   - **build output**: `.next`
   - **root directory**: `portfolio`
5. deploy

### vercel (alternative)

```bash
npm install -g vercel
vercel
```

## customization

### personal info
edit `app/page.tsx`:
- **line 99-100**: terminal prompt
- **line 103-106**: bio text
- **line 109-125**: skill badges
- **line 149-154**: current activities
- **line 172**: skills array
- **line 194**: email

### social links
- **github**: line 125, 197
- **twitter**: line 133, 203
- **linkedin**: line 209

### metadata
edit `app/layout.tsx`:
- **line 5**: page title
- **line 6**: meta description

### colors
edit `app/globals.css`:
- light mode: lines 12-28
- dark mode: lines 63-81

## design philosophy

- **brutalist minimalism**: no visual fluff
- **terminal aesthetic**: command-line inspired
- **information density**: tiny fonts, tight spacing
- **monospace everything**: code-like typography
- **sharp edges**: no rounded corners
- **lowercase**: hacker culture

## license

mit

---

built with ❤️ and monospace fonts