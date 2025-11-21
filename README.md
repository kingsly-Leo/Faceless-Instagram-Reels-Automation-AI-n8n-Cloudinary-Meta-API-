Faceless Instagram Reels Automation using AI & n8n

This project automates the complete creation and publishing of faceless aesthetic Instagram Reels using n8n, Pexels API, Cloudinary, and the Instagram Graph API.
The system generates reels automatically by fetching random aesthetic video clips, adding subtitles, overlay text, background audio, and posting them directly to an Instagram account—without any manual editing.

This solution is ideal for automation creators, content marketers, faceless theme pages, and AI-powered social media workflows.

✨ Key Features

Automated Clip Selection
Retrieves random aesthetic or faceless-style clips from Pexels API based on dynamic prompts.
(Implemented using HTTP Request node) 

Faceless instagram Reels Automa…

.

Dynamic Hashtag & Caption Generation
Captions are built automatically using:

the selected clip category

custom hashtags

call-to-action text
(Handled in the “Pick Clip” Function node) 

Faceless instagram Reels Automa…

.

Cloudinary Video Processing

Fetches video from Pexels

Uploads to Cloudinary

Adds background audio

Adds styled subtitles

Crops to 9:16 Reel format

Applies overlays and aesthetic color themes
(Implemented in Transform URL function) 

Faceless instagram Reels Automa…

.

Random Subtitle System
If transcript extraction fails, a random motivational or aesthetic quote is added.

Instagram Reels Auto-Publish
Uses the Instagram Graph API to:

Upload media container

Wait for processing

Publish the Reel

Retrieve the permalink
(Nodes: IG Create Media → Wait → IG Publish) 

Faceless instagram Reels Automa…

.

🧩 System Architecture

n8n Workflow

Start

Pexels API Search → fetch 15 aesthetic clips

Pick Clip Function → choose best clip + generate caption

Cloudinary Upload → fetch remote video

Build Transform URL Function →

Add subtitles

Add soundtrack

Add overlay text

Create final downloadable Reel URL

Instagram Create Media

Wait 15 seconds

Instagram Publish

Extract Permalink

This creates a fully autonomous Reel generator.

🛠️ Technologies Used
APIs

Pexels Videos API

Cloudinary Upload & Transform APIs

Meta Instagram Graph API v23.0

Automation Platform

n8n (workflow automation with function nodes)

AI & Logic

Random prompt selection

Auto-captioning

Subtitle overlay engine

Random soundtrack engine

📂 Workflow File

Faceless instagram Reels Automations.json – Complete n8n workflow ready for import.
(Contains all nodes and transformation logic) 

Faceless instagram Reels Automa…

.

🚀 How to Use This Project

Import the JSON workflow in n8n
Go to n8n Dashboard → Import Workflow.

Add your API credentials

Pexels API Key

Cloudinary Cloud Name + Upload Preset

Instagram Graph API Access Token
(Replace placeholders in HTTP Request nodes)

Adjust Prompts (Optional)
Edit the prompts list inside “Pexels Search” node to match your niche.

Run the workflow
Your Instagram account will publish reels automatically.
