An AI-powered marketing team dashboard that lets one person 
operate at the scale of a full marketing team.

> One prompt. Six AI agents. A full marketing campaign in seconds.

Built as a prototype to demonstrate how one person can operate 
at the scale of a full marketing team using AI.

## What it does

Describe any product → 6 specialist AI agents activate sequentially:

| Agent | Output |
|-------|--------|
| 🎯 CMO | 3-bullet marketing strategy |
| ✍️ Copywriter | Headline + tagline |
| 🔍 SEO Specialist | 5 target keywords with intent labels |
| 📱 Social Media Manager | Posts for LinkedIn, X, and TikTok |
| 📧 Email Marketer | Subject line + preview text |
| 📊 Analytics Manager | 4 KPIs to track |

## Built with

- [Lovable](https://lovable.dev) — frontend
- [Anthropic Claude API](https://anthropic.com) — powers each agent
- React + TailwindCSS

## Lovable prompts used to build this

**Initial prompt:**
> "Build a marketing team AI dashboard. It has a sidebar with team 
> members: CMO, Copywriter, SEO Specialist, Social Media Manager, 
> Email Marketer, and Analytics Manager. Each has an avatar and a 
> status indicator (idle/thinking/done). At the top there's a text 
> input where I type a product description and a Run Campaign button. 
> When clicked, each agent card activates one by one and displays 
> their specific output — CMO shows a strategy summary, Copywriter 
> shows a headline and tagline, SEO Specialist shows 5 target keywords, 
> Social Media Manager shows 3 post ideas, Email Marketer shows a 
> subject line and preview text, Analytics Manager shows KPIs to track. 
> Use a cobalt blue (#5B7FFF) and white theme, modern SaaS look, 
> clean card layout."

**API integration prompt:**
> "Connect each agent to the Anthropic Claude API using model 
> claude-haiku-4-5-20251001. When the user clicks Run Campaign, 
> call the API for each agent sequentially with their own system 
> prompt. Show thinking... status while each agent runs, then Done 
> when complete. The API key should be entered by the user in a 
> settings field."


Note: 
You have to get your own Anthropic API key, follow the steps below:

Go to console.anthropic.com

Sign in / create an account
Click "API Keys" in the left sidebar
Click "Create Key"
Copy it immediately — it only shows once
Paste key in Settings
Describe your product and hit Run Campaign

## Try it yourself : App Link : https://allhandsondeck.lovable.app/
