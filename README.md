# weddingsma.com — Amikam Yalovetzky, Wedding Officiant

## Files

```
/
├── index.html       — Main one-pager (home)
├── gallery.html     — Ceremony photo gallery
├── images/          — Drop your photos here
└── README.md
```

## Adding Photos to the Gallery

1. Put your image files in the `images/` folder (JPG or WebP recommended).
2. Open `gallery.html` and replace a placeholder block like this:

```html
<!-- BEFORE (placeholder) -->
<div class="gallery-placeholder" style="min-height:320px">
  <span class="ph-icon">🕍</span>
  <span>Chuppah photo 1</span>
</div>

<!-- AFTER (real photo) -->
<div class="gallery-item" data-filter="chuppah" data-caption="Under the Chuppah" data-location="Boston, MA">
  <img src="images/ceremony-01.jpg" alt="Couple under the chuppah" loading="lazy" />
  <div class="gallery-overlay">
    <div class="gallery-caption">
      <strong>Under the Chuppah</strong>Boston, MA
    </div>
  </div>
</div>
```

**Filter categories:** `chuppah` · `ritual` · `couple` · `celebration`

## Deploy to GitHub Pages

1. Create a new repo at github.com (name it `weddingsma.com` or any name)
2. Upload all files (or push via Git)
3. Go to Settings → Pages → Source: **main branch / root**
4. Your site goes live at `https://yourusername.github.io/reponame`

## Connect weddingsma.com via Netlify

1. Push this repo to GitHub
2. Log into netlify.com → Add new site → Import from GitHub → pick this repo
3. Deploy — Netlify auto-deploys on every push to main
4. In Netlify: Site Settings → Domain Management → Add `weddingsma.com`
5. In GoDaddy DNS: set A record `@` → `75.2.60.5`, CNAME `www` → `weddingsma.com`
6. Back in Netlify: Enable HTTPS (free SSL auto-provisioned)
