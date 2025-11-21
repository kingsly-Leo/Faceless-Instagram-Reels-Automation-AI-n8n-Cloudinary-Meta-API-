📚 Repository Overview
Repository: kingsly-Leo/Faceless-Instagram-Reels-Automation-AI-n8n-Cloudinary-Meta-API-
Purpose:
Automates the entire process of generating, stylizing, captioning, and publishing faceless, aesthetic Instagram Reels automatically leveraging AI, the n8n workflow automation platform, Pexels API, Cloudinary, and the Instagram Graph API.

✨ Features
Automated Clip Selection: Pulls random, aesthetic/faceless videos from Pexels via API based on dynamic prompts.
Dynamic Hashtag & Captioning: Captions and hashtags are auto-generated using the clip’s category, custom tags, and CTAs.
Cloudinary Video Processing: Handles fetching, uploading, applying audio, styling subtitles, cropping, overlays, and color themes.
Random Subtitle System: Random motivational/aesthetic quote is used if transcript extraction fails.
Instagram Reels Auto-Publish: Handles uploading, processing, publishing, and extracting permalinks—all via the Instagram Graph API.
Fully Autonomous Workflow: No manual intervention required; the system loops through discovery, transformation, and publishing.
🧩 System Architecture
n8n Workflow Steps:

Start
Pexels API Search → fetch 15 aesthetic/faceless clips
Pick Clip Function → select best, generate smart caption
Cloudinary Upload
Transform URL Function → add subtitles, soundtrack, overlays, crop, style
Instagram Create Media
Wait (process video)
Instagram Publish
Permalink Extraction
🛠️ Technologies
APIs:

Pexels Videos API
Cloudinary Upload/Transform
Instagram Graph API v23.0
Automation & Logic:

n8n workflow engine + function nodes
Random prompt/clip/soundtrack selection
Auto-captioning & overlay
Subtitle system
📂 Workflow File
Faceless instagram Reels Automations.json:
Complete n8n workflow file for direct import (includes nodes, logic, transformations).
🚀 Quick Start
Import: Use n8n's dashboard to import the provided workflow JSON.
Add API Keys:
Pexels API Key
Cloudinary Credentials
Instagram Graph API Access Token
Customize:
Prompts (in Pexels Search node)
Subtitle font/colors, overlays, soundtrack, etc.
Run Workflow:
Fully automated Reels generation & publishing.
🔧 Customizations
Change subtitle styling or colors
Expand nature/faceless prompts
Substitute or expand soundtrack library
Adjust cropping, overlays, analytics, etc.
📌 Notes
Requires Instagram Business/Creator account (linked to Facebook Page)
Needs Instagram Graph API permissions
Free Cloudinary tier suffices for moderate usage
