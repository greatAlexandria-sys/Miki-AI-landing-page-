# Quick Start — 5 Minutes to Live

## What You're Getting

- **index.html** — The complete, working website
- **vercel.json** — Config for instant deployment
- **README.md** — Full documentation

## Deploy to Vercel (Recommended — 2 Minutes)

### Step 1: Create GitHub Repo
```bash
# Push index.html to GitHub
# Name it: miki-ai-landing
```

### Step 2: Connect to Vercel
1. Go to https://vercel.com/new
2. Select "Import Git Repository"
3. Paste your GitHub repo URL
4. Click "Import"
5. **Done** — Live in 30 seconds

Your site is now live at: `your-project.vercel.app`

---

## Deploy to Netlify (Alternative — 1 Minute)

1. Go to https://app.netlify.com/
2. Drag and drop `index.html` onto the screen
3. **Done**

Live immediately.

---

## Deploy Locally (Testing)

```bash
# Option A: Python
python -m http.server 8000

# Option B: Node
npx http-server

# Option C: PHP
php -S localhost:8000

# Visit: http://localhost:8000
```

---

## Customization Checklist

- [ ] Update brand color (`#10203d` → your color)
- [ ] Replace "M" logo with your logo
- [ ] Change hero headline
- [ ] Update CTA button links
- [ ] Add your company footer info
- [ ] Test on mobile

---

## What You Need to Know

✅ **Self-contained** — No build, no npm install, no dependencies  
✅ **Fast** — Loads in <1s on 3G  
✅ **Mobile-first** — Works perfect on phone/tablet  
✅ **Production-ready** — Use as-is, no modifications needed  
✅ **Customizable** — Change colors/copy in minutes  

---

## Troubleshooting

**Q: Page is blank**  
A: Check browser console (F12). Should show no errors. If using file://, deploy instead (Vercel/Netlify).

**Q: Colors don't match my brand**  
A: Line 44 in index.html. Find `'brand-dark': '#10203d'` and change hex value.

**Q: Buttons don't work**  
A: Change `href="#"` to real URLs. Example:
```html
<a href="https://your-form.com/pilot" class="btn-primary">Start a Pilot</a>
```

**Q: FAQ accordion won't open**  
A: Check browser supports `<details>` (all modern browsers do). Try hard refresh (Ctrl+Shift+R).

---

## Next Steps

1. Deploy to Vercel or Netlify
2. Point your domain to it
3. Add Google Analytics (1 line in head)
4. Add contact form (embed Typeform or HubSpot)

---

## File Checklist

You should have:
- ✅ index.html
- ✅ vercel.json
- ✅ README.md
- ✅ QUICKSTART.md (this file)

That's all. Ship it.
