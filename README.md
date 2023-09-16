## Tool Description

A chat interface that allows users to upload PDF/DOCX documents and and chat with them using ChatGPT as the large language model.

https://user-images.githubusercontent.com/4984377/233852126-6828f7b6-cfc3-485c-a893-c2ce9e6b345f.mp4

## Installation

1. Make sure you ave installed Node v18 or later
2. Download the tool's repository using the command:

```bash
git clone git@github.com:ciocan/langchain-chat-with-documents.git
```

3. Move to the tool's directory and install the tool

```bash
cd langchain-chat-with-documents
npm install
```

4. Copy the .env.example into .env file and add the following variables:

```bash
WEAVIATE_HOST= # do not use https:// just the domain like bellingcat-xxx.weaviate.network
WEAVIATE_API_KEY=

# cloudflare r2
CLOUDFLARE_ACCOUNT_ID=
CLOUDFLARE_SECRET_KEY=
CLOUDFLARE_SECRET_ACCESS_KEY=

# open ai key
OPENAI_API_KEY=
```

Weaviate is an open source vector database where the documents are vectorized and indexed. You can install it locally or use their [free cloud](https://console.weaviate.cloud/).

Cloudflare R2 is a object storage solution compatible with AWS S3. They have a free tier of 10gb. [More info](https://www.cloudflare.com/products/r2/)

Signup for an OpenAI API key [here](https://platform.openai.com/)

1. Start the tool

```bash
npm run dev
```