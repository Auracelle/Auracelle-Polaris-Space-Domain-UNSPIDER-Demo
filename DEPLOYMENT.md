DEPLOYMENT.md
Auracelle Polaris · UN-SPIDER Edition · GitHub Pages Deployment Guide

## Quick Start: Deploy in 5 Minutes

### Prerequisites
- GitHub account (free)
- 5 minutes of time

### Steps

1. **Create a new GitHub repository**
   - Go to [github.com/new](https://github.com/new)
   - Repository name: `Auracelle-Polaris-UN-SPIDER` (or your preferred name)
   - Description: "Auracelle Polaris: UN-SPIDER Edition Space Governance Wargaming"
   - Set to **Public** (required for GitHub Pages)
   - Do NOT initialize with README, .gitignore, or license

2. **Clone the repository locally**
   ```bash
   git clone https://github.com/YOUR-USERNAME/Auracelle-Polaris-UN-SPIDER.git
   cd Auracelle-Polaris-UN-SPIDER
   ```

3. **Add the files**
   Copy these files to your local repository folder:
   - `index.html` (the main Polaris simulation)
   - `README.md`
   - `LICENSE`
   - `CITATION.md`
   - `SECURITY.md`
   - `.nojekyll` (hidden file — tells GitHub Pages to skip Jekyll processing)

4. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit: Auracelle Polaris UN-SPIDER Edition"
   git push -u origin main
   ```

5. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click **Settings** (top menu)
   - Click **Pages** (left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Select **main** branch and **/root** folder
   - Click **Save**
   - GitHub will display your live URL (typically `https://YOUR-USERNAME.github.io/Auracelle-Polaris-UN-SPIDER/`)

6. **Verify Deployment**
   - Visit your live URL in a browser
   - You should see the "POLARIS - SPACE DOMAIN" login screen
   - Log in with email + `UNSPIDER2026!`
   - Simulation should load immediately

**Total time**: < 5 minutes

---

## GitHub Pages Deployment Details

### What Happens When You Deploy

1. **GitHub builds the site** automatically (< 1 minute)
2. **Files are served at your GitHub Pages URL** (e.g., `https://username.github.io/repo-name/`)
3. **Updates are instant** — push new changes and they deploy within 30 seconds

### Live URL Formats

**Standard GitHub Pages URL**:
```
https://YOUR-USERNAME.github.io/Auracelle-Polaris-UN-SPIDER/
```

**Custom domain** (optional):
```
https://polaris.yourdomain.com
```
(See "Custom Domain Setup" section below)

### Files Required for GitHub Pages

These files are included in this package:

| File | Purpose |
|------|---------|
| `index.html` | Main Polaris simulation (playable) |
| `README.md` | Documentation (displayed on GitHub) |
| `LICENSE` | Open source license |
| `CITATION.md` | Academic citation formats |
| `SECURITY.md` | Security policy & responsible disclosure |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing |

All files should be in the **repository root** (not in subfolders).

---

## For UN-SPIDER Conference Organizers

### Pre-Conference Checklist

- [ ] Deploy repository to GitHub Pages
- [ ] Test login with `UNSPIDER2026!` access code
- [ ] Share live URL with conference participants (via website, email, QR code, etc.)
- [ ] (Optional) Customize access code for your event
- [ ] Document the URL and access code in conference materials
- [ ] Test on multiple browsers (Chrome, Firefox, Safari, Edge, mobile)

### During the Conference

#### Option A: Integrated into Session/Workshop

1. **Facilitator opens Polaris** on projection screen
2. **Participants log in individually** on their own devices (laptops, tablets)
3. **Play Scenario 06** (Earth Observation Data Access Deadlock) — ~15-20 min
4. **Facilitated discussion**:
   - Why did unilateral moves fail?
   - How did the Contested Negotiation Table resolve deadlock?
   - What are the implications for real UN-SPIDER operations?
5. **Collect feedback** (optional: Google Form or post-conference survey)

#### Option B: Exhibit/Booth Simulation

1. **Booth staff demonstrate Polaris** on a tablet or laptop
2. **Visitors get a 5-minute "quick play"** (1-2 moves, focusing on key insights)
3. **QR code** on booth materials links to live platform for later play
4. **Handouts** include access code, URL, and key findings from Scenario 06

#### Option C: Self-Paced Learning

1. **Share URL** in conference materials, sessions, and website
2. **Participants play independently** before/after conference
3. **No scheduled time required** — fits participant schedules
4. **Post-conference**: Gather feedback and usage analytics

### Sharing the Platform

**Email template** for participants:

> **Subject**: Play Polaris: Space Governance Wargaming at UN-SPIDER 2026
>
> Dear Conference Participant,
>
> As part of the 11th Annual UN-SPIDER Conference on Resilient Futures, we invite you 
> to play **Auracelle Polaris**, an interactive wargaming simulation focused on Earth 
> Observation data governance and disaster risk reduction.
>
> **Launch Polaris**: [INSERT YOUR URL]  
> **Access Code**: `UNSPIDER2026!`
>
> **Duration**: ~20 minutes per scenario (play at your own pace)
>
> **What to Expect**:
> - 6 space governance crisis scenarios
> - Real-time Agentic AI stress-testing of your policy choices
> - Governance-Resilience diagnostic scoring
> - Actionable recommendations for institutional reform
> - Specific focus on Earth Observation data access (Scenario 06 for UN-SPIDER participants)
>
> **Why Play?**
> Polaris stress-tests your understanding of how space governance institutions handle 
> pressure. You'll see why multilateral negotiation tables resolve deadlock that unilateral 
> moves cannot, and how to balance speed (resilience) with legitimacy (governance).
>
> Questions? See the full documentation at the platform or contact grace.evans@auracelle.ai
>
> Warm regards,  
> UN-SPIDER Conference Team

**QR Code**: Generate a QR code linking to your live URL (free via qr-server.com)

---

## Customizing the Access Code

**To change the access code for a different event:**

1. **Open `index.html`** in a text editor
2. **Find line ~1005** (search for: `if(code === 'UNSPIDER2026!')`)
3. **Replace `'UNSPIDER2026!'`** with your custom code
4. **Save the file** and push to GitHub:
   ```bash
   git add index.html
   git commit -m "Update access code for [EVENT NAME]"
   git push
   ```
5. **Live URL updates automatically** within 30 seconds

**Example custom codes**:
- `WSIS2027PARIS!`
- `UNOOSA2026!`
- `UNDRR_SPACE!`
- `ARCHANGEL2026!` (for private/restricted access)

---

## Custom Domain Setup (Optional)

To use a custom domain (e.g., `polaris.un-spider.org`):

1. **Register a domain** (if you don't already have one)
2. **Update your DNS records** to point to GitHub Pages:
   - Add a `CNAME` record pointing to `YOUR-USERNAME.github.io`
   - OR add `A` records pointing to GitHub's IP addresses (see [GitHub docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site))
3. **In your repository**:
   - Go to **Settings** → **Pages**
   - Under "Custom domain", enter your domain name (e.g., `polaris.un-spider.org`)
   - Click **Save**
   - GitHub will verify the domain (may take a few minutes)
4. **Enforce HTTPS** (recommended):
   - Once domain is verified, check "Enforce HTTPS" in Pages settings

**Time to deploy**: 15-30 minutes (mostly waiting for DNS propagation)

---

## Monitoring & Analytics

### GitHub Analytics

GitHub Pages provides basic traffic data:
- Go to **Settings** → **Pages**
- You'll see page views and referrers

### Custom Analytics (Optional)

If you want to track engagement without collecting user data:

**Option 1: Plausible Analytics** (privacy-friendly)
- Add one line of script to `index.html` (before `</body>`)
- No cookies, GDPR-compliant
- Costs ~$10/month

**Option 2: Simple Visitor Counter** (no data collection)
- Services like `countapi.xyz` or `hits.seeyoufarm.com`
- Shows total visits, nothing else
- Free

**NOT recommended**: Google Analytics, Facebook Pixel, or other tracking (conflicts with Polaris's privacy-first design)

---

## Troubleshooting

### "Page not loading" or "404 error"

**Solution**: 
- Check that your repository is **Public** (not Private)
- Verify GitHub Pages is **enabled** in Settings → Pages
- Wait 1-2 minutes for GitHub to build the site
- Clear your browser cache and reload
- Try a different browser to rule out caching issues

### "Login works but simulation doesn't appear"

**Solution**:
- This was a bug in earlier versions — **already fixed** in this package
- If you're using an updated version and still see this:
  - Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
  - Clear browser cache
  - Try in private/incognito window

### "Access code not working"

**Solution**:
- Verify you're using exactly: `UNSPIDER2026!` (with exclamation mark)
- Check CAPS LOCK is off
- If you customized the code, make sure you pushed the changes:
  ```bash
  git status  # Check if index.html shows as modified
  git push    # Push changes to GitHub
  ```

### "Page loads very slowly"

**Solution**:
- First load: Normal (4.4 MB file downloading)
- After that: Should load from browser cache (instant)
- If still slow: Check your internet connection
- GitHub Pages servers are global; should be fast from any location

---

## Security Considerations for Deployment

### For UN-SPIDER Use

- Polaris is **unclassified** and safe for general government/UN agency use
- No need for special hosting or security infrastructure
- GitHub Pages is trusted by governments, universities, and research institutions worldwide
- **HTTPS is automatic** (GitHub Pages enforces it)

### Data Privacy

- Polaris **does NOT send any data** to external servers
- Player emails are stored locally only (sessionStorage)
- No tracking, analytics, or third-party integrations
- **Participant privacy is preserved**

---

## Updates & Maintenance

### To Update Polaris

1. **Download new version** from GitHub
2. **Replace `index.html`** with the new version
3. **Push to your repository**:
   ```bash
   git add index.html
   git commit -m "Update Polaris to [VERSION NUMBER]"
   git push
   ```
4. **Live URL updates automatically** within 30 seconds

### Staying Current

- Watch this repository for updates: Click **Watch** → **Releases only**
- Subscribe to security advisories (see SECURITY.md)

---

## Support & Questions

For deployment help, technical issues, or questions about UN-SPIDER integration:

📧 **Email**: grace.evans@auracelle.ai  
🔗 **GitHub Issues**: [This repository's Issues tab]  
🔗 **Platform**: https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public

---

## Checklist: Pre-Launch

Before you go live with Polaris:

- [ ] Repository is created and files are uploaded
- [ ] GitHub Pages is enabled in Settings
- [ ] Live URL is working (test in browser)
- [ ] Login works with access code
- [ ] Simulation loads after login (no refresh needed)
- [ ] All 6 scenarios are selectable
- [ ] Moves can be played and AI responses appear
- [ ] Prompt "What's your next move?" appears after each response
- [ ] Test on mobile device (if applicable for your audience)
- [ ] README is publicly visible on GitHub
- [ ] LICENSE, CITATION.md, SECURITY.md are accessible
- [ ] URL is shared with participants (email, website, QR code)
- [ ] Access code is documented in conference materials
- [ ] (Optional) Custom domain is set up and working

---

**You're ready to launch Polaris for UN-SPIDER 2026!**

Questions? Email: grace.evans@auracelle.ai

---

Version 1.0 | June 2026
