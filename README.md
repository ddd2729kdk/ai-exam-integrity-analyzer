AI Exam Integrity Analyzer 
An AI-powered web tool that analyzes student exam answers for potential academic dishonesty.
/////

What it does
Paste up to 3 student answers into the tool
AI analyzes each answer for suspicious patterns:
Similarity between answers (copy-paste detection)
Unusual vocabulary or phrasing
AI-generated writing style
Structural patterns that suggest cheating
Outputs a Risk Score (0–100%) for each student
Provides a detailed explanation of why each score was given
Color-coded results:  🟢 Low / 🟡 Medium / 🔴 High risk
/////

How to run
Option 1 — Just open the file 
Download or clone this repository
Open index.html in any browser (Chrome, Firefox, Edge)
Enter your Anthropic API key
Paste student answers and click Analyze

Option 2 — Clone with Git
git clone https://github.com/Y_U/ai-exam-integrity-analyzer.git
cd ai-exam-integrity-analyzer
open index.html
/////

Getting an API Key
Go to console.anthropic.com
Sign up for a free account
Go to API Keys → Create Key
Paste the key into the app (starts with sk-ant-...)
/////

Tech Stack
Technology  --   Purpose
HTML / CSS / JavaScript  --   Frontend (no frameworks needed)
Anthropic Claude API  --   AI analysis engine
Claude Sonnet 4 model  --   Prompt engineering + structured output
Google Fonts  --   Typography (Space Mono + DM Sans)
/////

Prompt Engineering
The core of this project is a carefully designed prompt that instructs Claude to:
1.Act as an academic integrity analyst
2.Compare answers for linguistic similarity
3.Detect AI-generated patterns
4.Return structured JSON with scores and explanations

You are an academic integrity analyst. Analyze the following 
student exam answers for potential cheating, copying, or 
AI-generated content...
/////

Project Structure
ai-exam-integrity-analyzer/
├── index.html     ← entire application (HTML + CSS + JS)
└── README.md      
