This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app). It has an implementation of Copilotkit using Agents in a Todo application.

For more information about the Agent used, read its [README.md](agent/README.md).

## Getting Started

There are two main applications to be aware of - the UI (Next.js app) and the Agent (FastAPI served LangGraph).

### Environment Variables
The Agent utilized in this project uses OpenAI and Tavily. Create a `.env` in [agent](./agent/) and populate it
with the following.

```
OPENAI_API_KEY=<your_opanai_api_key>
TAVILY_API_KEY=<your_tavily_api_key>
```

### Starting the server
There are two processes necessary here. Included is a `all` script that will run both but you have to install their
necessary dependencies first.

1. `npm install`
2. `cd ./agent && poetry install`
3. `npm run all`

Open [http://localhost:3000](http://localhost:3000) with your browser to see the page.
