SECURITY.md
Auracelle Polaris · UN-SPIDER Edition · Security Policy & Responsible Disclosure

## Security Overview

Auracelle Polaris UN-SPIDER Edition is a browser-based educational and research 
wargaming simulation designed for governance analysis and decision-making under 
pressure. The simulation runs entirely client-side in your browser and does not 
collect, store, or transmit personal data beyond session management.

Security and responsible use are critical for maintaining trust with UN-SPIDER 
participants, government partners, and research institutions.

---

## Browser Security & Privacy

### What Polaris Does NOT Do

✓ Does NOT collect, store, or transmit user data to external servers
✓ Does NOT require authentication beyond a simple access code
✓ Does NOT use cookies, tracking technologies, or analytics
✓ Does NOT require network connectivity after initial page load
✓ Does NOT execute external code or contact remote servers
✓ Does NOT use third-party JavaScript libraries (except Google Fonts for typography)
✓ Does NOT store gameplay history, simulation outputs, or user email addresses persistently
✓ Does NOT profile players or use behavioral data for any purpose

### Data Storage

**Session-based only** (cleared when browser is closed):
- User email address: Stored in `sessionStorage` (browser-specific, not persisted)
- Access timestamp: Stored in `sessionStorage` for session validation
- Gameplay state: Stored in JavaScript variables in memory only

**Your browser's JavaScript sandbox** protects the system from most attacks:
- JavaScript runs in a sandboxed execution environment
- Cannot access your file system, operating system, or other applications
- Cannot modify system settings or install software
- Cannot access data from other websites

### Recommendations for Secure Use

- Keep your browser up to date with the latest security patches
- If on a shared or untrusted device, consider browsing in a private/incognito window
- Review your browser's privacy settings before accessing Polaris
- Clear your browser history and cache after playing if desired (though no persistent data is stored)

---

## Access Control & Conference Security

### Access Code

- **Credential**: Simple password (`UNSPIDER2026!`) to gate access to the simulation
- **Purpose**: Limits unauthorized access; allows conference organizers to track engagement
- **Customization**: Conference hosts can change the access code (see README.md for instructions)
- **NOT for production authentication**: This is a lightweight conference gating mechanism, not an authentication system for sensitive operations

### Session Management

- Sessions are browser-specific and tied to `sessionStorage`
- Sessions persist for the duration of the browser window (cleared when closed)
- No centralized session server or backend validation
- Each participant's session is independent

### For UN-SPIDER & Government Use

- Polaris is suitable for **unclassified** research, capacity building, and educational use
- **NOT recommended** for classified or sensitive government decision-making
- **NOT designed** for real operational scenarios; it is a pedagogical stress-testing tool
- Participants should treat simulation outputs as learning artifacts, not intelligence

---

## Responsible Use Policy

Auracelle Polaris is intended for:

✓ Academic research on space governance and disaster risk reduction
✓ Educational instruction in policy analysis, wargaming methodology, and strategic decision-making
✓ Government and allied institution policy exploration and capacity building
✓ UN agencies and UNOOSA programs conducting governance research
✓ Think tank and non-profit research on space law and geopolitics
✓ Conference workshops, simulations, and training exercises
✓ Curriculum integration in universities and research centers

### Prohibited Uses

✗ Commercial sale or licensing without explicit written permission
✗ Reverse-engineering or attempting to extract proprietary methodology without authorization
✗ Unauthorized distribution or modification
✗ Use by adversarial or non-aligned states without written permission (see LICENSE)
✗ Misrepresentation of simulation outputs as real intelligence or predictions
✗ Integration into automated decision-making systems without human oversight
✗ Deployment for actual space operations or real-world crisis management
✗ Use for propaganda, disinformation, or geopolitical manipulation

---

## Reporting Security Issues

If you discover a security vulnerability or issue with Auracelle Polaris, please 
report it **responsibly and confidentially**:

### DO NOT:
- Post the vulnerability publicly in GitHub Issues
- Share vulnerability details on social media or forums
- Exploit the vulnerability for any purpose

### DO:
Contact Grace-Alice Evans directly:

📧 **Email**: grace.evans@auracelle.ai  
🔗 **LinkedIn**: https://www.linkedin.com/in/grace-alice-evans-5a9632a3

### Please Include:

1. Description of the security issue
2. Steps to reproduce (if applicable)
3. Potential impact and severity
4. Suggested remediation (if you have one)
5. Your name and contact information (optional but appreciated)

### Response Timeline:

- Acknowledgment: Within 48 hours
- Investigation: Within 1 week
- Remediation/disclosure decision: Within 2 weeks
- Public disclosure or security advisory: Coordinated with reporter

We appreciate your responsible disclosure and will credit you appropriately in any 
security advisories if you wish.

---

## Known Limitations & Disclaimers

### Simulation vs. Reality

- Polaris is a **decision-support tool**, not a prediction engine
- Simulation outputs reflect **programmed scenario logic and game theory**, not machine learning or real data
- **Scenarios are simplified representations** of complex geopolitical situations
- Real-world space governance involves far more nuance, uncertainty, and dynamic variables than any simulation can capture
- Players should treat Polaris as a **learning tool and stress-testing aid**, not as a substitute for:
  - Expert policy analysis by space law and governance specialists
  - Real intelligence assessments by government agencies
  - Multilateral negotiation and diplomatic processes
  - Operational decision-making in actual crises

### Agentic AI Response Logic

- **Deterministic, rule-based** (not machine-learned from real data)
- Based on **game theory principles** (prisoner's dilemma, coalition formation, etc.)
- Reflects **documented governance doctrines** (US space policy, Chinese space doctrine, etc.)
- **NOT** trained on classified intelligence or real-world decision data
- Outcomes are **illustrative**, not predictive

### Earth Observation Scenario Specificity

The UN-SPIDER scenario (Scenario 06) is based on:
- Real EO governance challenges (data access, sovereignty, capacity gaps)
- Existing mechanisms (International Charter on Space and Major Disasters)
- Published research on space-based disaster risk reduction
- WSIS and UNDRR policy documents
- Published reports from space agencies (NOAA, ESA, CNSA, JAXA, etc.)

However, it is **NOT**:
- A formal assessment of current UN-SPIDER operations
- A prediction of actual UN governance outcomes
- A validated model of real stakeholder behavior
- An authoritative guide for policy implementation

---

## Incident Response Plan

In the event of a security incident affecting the Polaris repository or GitHub Pages 
deployment:

1. **Immediate response**: Repository administrators will investigate
2. **User notification**: Security advisory published on GitHub Releases
3. **Mitigation**: Patched version deployed to GitHub Pages
4. **Communication**: Updates posted to README.md and SECURITY.md
5. **Transparency**: Full disclosure within 30 days (unless embargo requested)

### Reporting Incidents

For incidents affecting conference operations, GitHub deployment, or mass access issues:

📧 grace.evans@auracelle.ai (urgent)

Include:
- Description of the incident
- When it was discovered
- Systems/users affected
- Any error messages or logs

---

## Third-Party Code & Dependencies

### External Resources Used

**Google Fonts (CSS)**:
- URL: `https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&family=Space+Mono:wght@400;700&display=swap`
- Purpose: Typography/styling only (no JavaScript execution)
- Privacy: See [Google Fonts Privacy Policy](https://policies.google.com/privacy)
- Fallback: System fonts used if Google Fonts unavailable

### NO External JavaScript Libraries

Polaris is written in **vanilla JavaScript** and does NOT use:
- jQuery, React, Vue, Angular, or other frameworks
- npm packages or package managers
- CDN-hosted libraries (except Google Fonts for typography)
- Third-party analytics, tracking, or telemetry

This minimizes attack surface and external dependencies.

### Why Vanilla JavaScript?

- **Security**: Reduces vulnerability exposure from third-party package vulnerabilities
- **Privacy**: No tracking or data collection from framework providers
- **Performance**: Smaller file size, faster load times
- **Stability**: No dependency compatibility issues or breaking updates
- **Accessibility**: Direct control over WCAG compliance and user experience

---

## Compliance & Standards

### WCAG 2.1 Level AA Accessibility

- Keyboard navigation support
- Screen reader compatible
- Color contrast ratios meet standards
- Semantic HTML for assistive technologies

### Data Protection

- **GDPR**: No personal data collection or retention
- **CCPA**: No data sales or third-party sharing
- **UN Data Protection Framework**: Compliant with UN privacy standards

### Browser Compatibility

- Chrome/Chromium 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## Suggestions for Improvement

If you have suggestions for improving Polaris's security, privacy, or responsible use 
practices, please reach out:

📧 grace.evans@auracelle.ai

We welcome feedback on:
- Security best practices
- Privacy enhancements
- Accessibility improvements
- Responsible AI usage guidelines
- Incident response procedures

---

## Questions?

For security inquiries, policy clarifications, or responsible disclosure:

📧 **Email**: grace.evans@auracelle.ai  
🔗 **Platform**: https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public  
🔗 **Suite**: https://auracelle.github.io/Auracelle-Suite-AI-Governance-Labs/

---

**Auracelle AI Governance Labs · Polaris UN-SPIDER Edition**  
Version 1.0 | June 2026

*Trust, transparency, and responsible governance are at the heart of Polaris.*
