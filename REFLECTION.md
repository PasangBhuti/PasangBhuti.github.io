
#Reflection 
## 1. the path of an HTTP request 
when a user types "https://pasangbhuti.github.io" the browser first performs a DNS lookup to translate the domain into GitHub's server IP address. It then sends an Http Get request to taht server asking for 'index.html'. the browser then rewuests any linked resources (styles.css',images) and renders the final page once everything loads, it renders the final page.

## 2. AI Attribution
**Prompt used**: "help me set up SSH authentication for GitHub"

**Logic error fixed**: I ran a command that still had the placeholder brackets
`pasanggurung' instead of my real GitHub username, which caused a 'zsh: bad pattern` error. I caught this and replaced it with my actual username.