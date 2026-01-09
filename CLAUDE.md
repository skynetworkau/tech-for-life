# Tech for Life - Project Context

## Overview
Year 12 Digital Literacy course for **Denmark Senior High School**, Western Australia.
16-week course covering AI, Cyber Safety, and Life Skills for school leavers.

## Deployment
- **Live Site:** https://tech-for-life.vercel.app (currently flagged by Google Safe Browsing - false positive)
- **GitHub:** https://github.com/skynetworkau/tech-for-life
- **Vercel Dashboard:** https://vercel.com/david-4021s-projects/tech-for-life

## TODO: Custom Domain Setup
Chrome is flagging the site as "dangerous" (false positive due to scam examples in Spot the Scam activity).

**To fix - add custom domain in Vercel:**
1. Go to https://vercel.com/david-4021s-projects/tech-for-life/settings/domains
2. Add your domain (e.g., `techforlife.teacherscreen.com.au`)
3. Add DNS records at your registrar:
   - Type: CNAME
   - Name: techforlife (or whatever subdomain)
   - Value: cname.vercel-dns.com
4. Wait for SSL certificate (automatic)

**Alternative:** Submit for Google review at:
https://safebrowsing.google.com/safebrowsing/report_error/?url=https://tech-for-life.vercel.app

---

## Course Structure

### Term 1: AI & Smart Tech (Weeks 1-8)
| Week | Title | Content |
|------|-------|---------|
| 1 | What is AI? | AI basics, types, how it works |
| 2 | AI for Study | NotebookLM, ChatGPT, study tools |
| 3 | AI Image & Design | Midjourney, Ideogram, Canva, Recraft |
| 4 | AI Ethics & Bias | Real bias examples, Amazon/healthcare cases |
| 5 | AI Misinformation | Deepfakes, detection tools |
| 6 | Your AI Policy | Creating personal AI guidelines |
| 7 | AI Prompt Engineering | RTCFCE framework, effective prompts |
| 8 | AI Showcase | Student presentations |

### Term 2: Cyber Safety (Weeks 9-13)
| Week | Title | Content |
|------|-------|---------|
| 9 | Spot the Scam | Australian scams, ACCC data |
| 10 | Password Security | Breaches, managers, 2FA |
| 11 | Digital Footprint | What employers find |
| 12 | Social Media & Future | Employer searches, reputation |
| 13 | Privacy Settings | Platform-specific guides |

### Term 3: Leaving School Ready (Weeks 14-16)
| Week | Title | Content |
|------|-------|---------|
| 14 | Life Admin Setup | myGov, TFN, Medicare, banking |
| 15 | Getting Work Ready | AI hiring, ATS, video interviews, resume hacks |
| 16 | Your Pathway | Uni, TAFE, apprenticeships, work - all options |

---

## Interactive Activities (9 total)

| Activity | Description | Features |
|----------|-------------|----------|
| Scam Hunter | Spot the scam quiz | 25+ scenarios, 3 game modes |
| Prompt Lab | AI prompt engineering | 15 challenges, RTCFCE builder |
| Footprint Finder | Digital footprint audit | 7 categories, privacy scoring |
| Password Lab | Password security demo | 8 modules, attack simulator |
| Life Admin Checklist | Track adulting progress | localStorage, achievements, 33 tasks |
| Resume Checker | Beat the ATS | Keyword matching, score gauge |
| Pathway Quiz | Find your best fit | 15 questions, personality results |
| Interview Practice | AI video interview sim | Webcam, recording, self-assessment |
| AI Tools Directory | 38+ AI tools | Search, filter, logos, links |

---

## Technical Details

- **Stack:** Pure HTML/CSS/JavaScript (no frameworks)
- **Hosting:** Vercel (static)
- **Storage:** localStorage for progress saving
- **APIs used:**
  - Google Favicon API for tool logos
  - MediaDevices API for webcam (Interview Practice)
  - MediaRecorder API for recording

## File Structure
```
Tech for Life/
├── index.html                 # Course hub
├── presentations/
│   ├── week1-what-is-ai/
│   ├── week2-ai-study/
│   ├── ... (16 total)
├── activities/
│   ├── spot-the-scam/
│   ├── ai-prompt-lab/
│   ├── digital-footprint/
│   ├── password-lab/
│   ├── life-admin-checklist/
│   ├── resume-checker/
│   ├── pathway-quiz/
│   └── interview-practice/
└── resources/
    └── ai-tools/
```

## Key Design Decisions
- Dark theme throughout (modern, engaging for Year 12)
- All examples use Australian/WA context
- Finance excluded (covered by Mandy Money)
- All pathways presented as equal (uni, TAFE, apprenticeships, work)
- Casual, friendly tone - "like advice from a cool older sibling"
- Practical "cheat codes" students can actually use

## Australian Resources Referenced
- my.gov.au, ato.gov.au, servicesaustralia.gov.au
- fairwork.gov.au (minimum wage, rights)
- tisc.edu.au (WA uni applications)
- training.gov.au, usi.gov.au
- seek.com.au, au.indeed.com
- WA universities: UWA, Curtin, Murdoch, ECU, Notre Dame
- WA TAFEs: North Metro, South Metro

---

## Future Improvements (if needed)
- Add more YouTube videos to presentations
- Create printable PDF versions of checklists
- Add teacher dashboard for tracking class progress
- Create quiz/assessment versions of activities
- Add more WA-specific content (Great Southern region jobs, local TAFEs)
