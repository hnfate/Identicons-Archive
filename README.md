# Identicons Archive

A complete, reproducible collection of GitHub’s default identicons.  
Every identicon is a deterministic 5×5-pixel sprite generated from a username hash, rendered here as both **SVG** (scalable) and **PNG** (420 × 420 px).

## Quick Start

```bash
git clone https://github.com/your-username/identicons-archive.git
cd identicons-archive
npm install     # only if you want to regenerate assets
```

#Folder Layout
```
identicons-archive
├── data/               # raw JSON mapping: username → hash
├── svg/                # 1:1 SVG files
├── png/                # 420×420 PNG exports
├── scripts/
│   └── generate.js     # Node script to render new identicons
├── LICENSE
└── README.md
```

#Usage
<img src="https://raw.githubusercontent.com/hnfate/identicons-archive/main/svg/octocat.svg" width="64" alt="octocat">

#Regenerate Everything
node scripts/generate.js --all

#Contributing
Open an issue for missing usernames or algorithm fixes.
Fork → branch → pull request.
Keep commits atomic; include the generated assets when relevant.
