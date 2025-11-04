# FDE Assignment — Text Analysis Automation

## Tools Used
- **n8n.cloud** for workflow automation
- **OpenAI API** for text analysis (summary/sentiment)
- **HTML, Tailwind CSS, JavaScript** for front-end UI

## Workflow Design
Webhook → HTTP Request (OpenAI) → Set → Webhook Response

## How it Works
1. User enters text and clicks a button.
2. Front-end sends POST request to n8n Webhook.
3. n8n passes text to OpenAI via API.
4. OpenAI returns summary/sentiment.
5. n8n sends back a clean JSON `{ "final_result": "..." }`.
6. Front-end displays the result.

## Deployment
- Hosted n8n workflow on n8n.cloud
- Front-end tested locally (can be hosted on Vercel or GitHub Pages)

## Files Submitted
- `n8n-workflow.json`
- `index.html`
- `documentation.md`
