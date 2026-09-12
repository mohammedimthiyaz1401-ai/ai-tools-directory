# ToolVerse - AI Tools Directory - AGENTS.md

## What
AI tools directory with 75+ tools across 12 categories. Search, filter by price/rating, find free alternatives.

## Tech Stack
- Single-page HTML/JS (no framework, no build step)
- Vanilla JS with TOOLS array in index.html
- Vercel hosting + GitHub Pages

## Key Files
- index.html - Everything (HTML + CSS + JS + tool data)
- All tools defined as JS objects in const TOOLS array (line ~162)

## How to Deploy
```
# Vercel
vercel --yes --prod

# GitHub Pages (auto on push)
git push origin main
```

## How to Add a Tool
Add object to TOOLS array in index.html:
```
{name:"ToolName",maker:"Company",icon:"emoji",iconBg:"#hex",cat:"Category",desc:"Description",price:"Free|Freemium|Paid|Waitlist",priceNote:"Pricing detail",rating:4.5,alt:"Free: alternative1, alternative2",url:"https://..."}
```

## Categories
AI Chat, Image Gen, Video Gen, Voice/TTS, Code, Writing, Productivity, Design, Marketing, Data, Research, Education

## Rules
- NO duplicate tools (check existing before adding)
- Price field must be exactly: "Free", "Freemium", "Paid", or "Waitlist"
- Rating: 1.0 to 5.0
- alt field: List free alternatives separated by commas

## Known Issues
- None currently active

## Email
futureintelligence4@gmail.com

## .gitignore
None needed (single HTML file, no secrets)
