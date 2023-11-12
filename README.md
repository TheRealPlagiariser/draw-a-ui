# draw-a-ui

This is an app that uses tldraw and the gpt-4-vision api to generate html based on a wireframe you draw.

![A demo of the app](./demo.gif)

This works by just taking the current canvas SVG, converting it to a PNG, and sending that png to gpt-4-vision with instructions to return a single html file with tailwind.

> Disclaimer: This is a demo and is not intended for production use. It doesn't have any auth so you will go broke if you deploy it.

## Getting Started

This is a Next.js app. To get started run the following commands in the root directory of the project. You will need an OpenAI API key with access to the GPT-4 Vision API.

> **Note**: The command `npm i node@lts` is intended for users with an older version of Node.js. If you're already running a recent LTS version of Node.js, you can skip this step.

```bash
echo "OPENAI_API_KEY=sk-your-key" > .env.local
npm i node@lts
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
