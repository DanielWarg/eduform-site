# Eduform.ai – AI-genererade ledarskapskurser

Detta är frontend-delen för Eduform.ai, ett SaaS för att skapa och leverera AI-genererade kurser. Fokus ligger initialt på ledarskap och utvecklas därefter modulärt.

## 🌟 Status

✅ Design och första version av startsida är färdig
✅ Hostad på Vercel – tillgänglig via [ai.postboxen.se](https://ai.postboxen.se)
✅ Använder Shadcn UI + Tailwind CSS + Next.js
✅ Anpassad för framtida kurspresentationer

---

## 🚀 Teknikstack

- **Next.js 14**
- **React**
- **Tailwind CSS**
- **shadcn/ui**
- **Vercel hosting**
- **TypeScript**

---

## 🔧 Kom igång lokalt

1. **Kloning:**
   ```bash
   git clone https://github.com/danielwarg/eduform-site.git
   cd eduform-site
   ```

---

## ✅ Projektlogg – Eduform.ai

Vi har:

- Initierat ett nytt Next.js-projekt via **V0.dev**, med UI-biblioteket **shadcn/ui** och **Tailwind CSS**.
- Anpassat startsidan grafiskt med inspiration från [postboxen.se](https://postboxen.se) och lagt till:
  - Hero med bakgrundsbild och CTA
  - Fördelar/kort (Cards)
  - Kursbibliotek (AI-genererade ledarskapskurser)
  - Testimonials
  - Avslutande CTA och footer
- Byggt med `app/page.tsx` som huvudfil.
- Pushat kod till Git (lokalt repo) och deployat med Vercel.
- Lagt till en **CNAME** på One.com: `ai.postboxen.se` → `cname.vercel-dns.com`.
- Vercel bekräftar **valid domain config** och `ai.postboxen.se` pekar korrekt mot deployment.

## ⚠️ Problem: Lokala servern fungerar inte

Vi har startat dev-servern med `npm run dev` (eller `pnpm dev`) – den svarar utan fel – men vi ser ingen sida när vi går till `http://localhost:3000`.

Möjliga orsaker:
- Cachen i webbläsaren, testa inkognito-läge.
- Fel i `app/page.tsx` som kraschar renderingen (ex. saknad import eller typfel).
- Felaktig installation (pröva `rm -rf .next node_modules && npm install`).
- Ingen `export default function Page()` i rätt mappstruktur.
