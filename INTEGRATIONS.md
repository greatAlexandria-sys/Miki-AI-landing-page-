# Easy Integrations

Add these snippets to `index.html` for common tools. Paste in the `<head>` section unless noted.

---

## Google Analytics 4

Add this to `<head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your GA4 ID from Google Analytics.

---

## HubSpot Form (Pilot Signup)

Replace any button with:

```html
<a href="https://share.hsforms.com/YOUR_FORM_ID" class="btn-primary">
  Start a Pilot
</a>
```

Or embed a pop-up form (add to `<head>`):

```html
<script charset="utf-8" type="text/javascript" src="//js.hsforms.net/forms/embed/v2.js"></script>
<script>
  hbspt.forms.create({
    region: "na1",
    portalId: "YOUR_PORTAL_ID",
    formId: "YOUR_FORM_ID"
  });
</script>
```

---

## Typeform (Contact/Pilot Form)

Replace button `href="#"` with:

```html
<a href="https://form.typeform.com/to/YOUR_FORM_ID" class="btn-primary">
  Start a Pilot
</a>
```

Or embed inline:

```html
<div data-tf-live="01ARZ3NDEKTSV4NNBESSVSLP41"></div>
<script src="//embed.typeform.com/next/embed.js"></script>
```

---

## Calendly (Meeting Scheduler)

Replace button with:

```html
<a href="https://calendly.com/YOUR_USERNAME" class="btn-primary">
  Schedule a Demo
</a>
```

Or embed pop-up:

```html
<button onclick="Calendly.initPopupWidget({url: 'https://calendly.com/YOUR_USERNAME'}); return false;" class="btn-primary">
  Schedule a Demo
</button>

<script src="https://assets.calendly.com/assets/external/widget.js"></script>
```

---

## Slack Notifications (When someone clicks CTA)

Add this to `<head>`:

```html
<script>
function notifySlack() {
  fetch('https://hooks.slack.com/services/YOUR/WEBHOOK/URL', {
    method: 'POST',
    body: JSON.stringify({
      text: '🚀 Pilot signup clicked!'
    })
  });
}
</script>
```

Then on button:

```html
<button class="btn-primary" onclick="notifySlack(); window.location='https://your-form.com'">
  Start a Pilot
</button>
```

Get webhook URL from Slack App → Incoming Webhooks.

---

## Intercom (Chat Widget)

Add to `<head>`:

```html
<script>
  window.intercomSettings = {
    api_base: "https://api-iam.intercom.io",
    app_id: "YOUR_APP_ID"
  };
</script>

<script async defer src="https://widget.intercom.io/widget/YOUR_APP_ID"></script>
```

---

## Crisp Chat (Alternative to Intercom)

Add to `<head>`:

```html
<script type="text/javascript">
  window.$crisp=[];
  window.CRISP_WEBSITE_ID="YOUR_WEBSITE_ID";
  (function(){d=document;s=d.createElement("script");s.src="https://client.crisp.chat/l.js";s.async=1;d.getElementsByTagName("head")[0].appendChild(s);})();
</script>
```

---

## Microsoft Clarity (Session Recording)

Add to `<head>`:

```html
<script type="text/javascript">
  (function(c,l,a,r,i,t,y){
    c[a]=c[a]||function(){(c[a].q=c[a].q||[]).push(arguments)};
    t=l.createElement(r);t.async=1;t.src="https://www.clarity.ms/tag/"+i;
    y=l.getElementsByTagName(r)[0];y.parentNode.insertBefore(t,y);
  })(window, document, "clarity", "script", "YOUR_PROJECT_ID");
</script>
```

---

## Open Graph / Social Share Preview

Add to `<head>` to customize how it looks on Twitter, LinkedIn, etc:

```html
<meta property="og:title" content="Miki AI — Retail Surveillance & POS Transaction Integrity" />
<meta property="og:description" content="Autonomous cross-referencing between surveillance video and point-of-sale logs to flag retail shrinkage instantly." />
<meta property="og:image" content="https://your-domain.com/og-image.jpg" />
<meta property="og:url" content="https://your-domain.com" />
<meta name="twitter:card" content="summary_large_image" />
```

---

## How to Find Your API Keys

| Tool | Where to Get |
|------|--------------|
| Google Analytics | analytics.google.com → Admin → Property ID |
| HubSpot | app.hubspot.com → Settings → Integrations |
| Typeform | typeform.com → My Forms → Get Link |
| Calendly | calendly.com → Settings → Scheduling Link |
| Slack Webhook | api.slack.com → Apps → Create → Incoming Webhooks |
| Intercom | app.intercom.com → Settings → API keys |
| Crisp | app.crisp.chat → Settings → Website ID |
| Clarity | clarity.microsoft.com → Projects → Tracking Code |

---

## Example: Full Setup

Hero section with GA + form embed:

```html
<section class="w-full bg-surface-light py-16 md:py-24">
  <div class="max-w-7xl mx-auto px-4 md:px-8 grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
    <div class="flex flex-col gap-6">
      <h1 class="text-headline-lg md:text-display font-semibold text-brand-dark leading-tight">
        What your cameras saw. What your till recorded. One answer.
      </h1>
      <button class="btn-primary" onclick="Calendly.initPopupWidget({url: 'https://calendly.com/your-username'}); return false;">
        Schedule a Demo
      </button>
    </div>
  </div>
</section>
```

That's it. Copy, paste, customize.
