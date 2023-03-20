# DocsGPT  🦖

## GPT based Documentation Assistant</strong>

<strong>DocsGPT</strong> is a solution that streamlines the process of finding information in project documentation. With its integration of the powerful <strong>GPT</strong> models, developers can easily ask questions about a project and receive accurate answers.
  
Say goodbye to time-consuming manual searches, and let <strong>DocsGPT</strong> help you quickly find the information you need. Try it out and see how it revolutionizes your project documentation experience. Contribute to its development and be a part of the future of AI-powered assistance.

## Project structure

- Application - flask app (main application)

- Extensions - chrome extension

- Scripts - script that creates similarity search index and store for other libraries.

## QuickStart

Please note: current vector database uses pandas Python documentation, thus responses will be related to it, if you want to use other docs please follow a guide below

Make sure you have python 3.10 or 3.11 installed

1. Navigate to `/application` folder
2. Install dependencies
`pip install -r requirements.txt`
3. Prepare .env file
Copy .env_sample and create .env with your openai api token
4. Run the app
`python app.py`

To start frontend

1. Navigate to `/frontend` folder
2. Install dependencies `npm install`
3. In the file  `.env.development` instead of `VITE_API_HOST = https://docsapi.arc53.com` use `VITE_API_HOST=http://localhost:5001`
4. Run the app `npm run dev`

Alternatively, you can use docker-compose to run the app via docker

1. From the root folder run `docker-compose build && docker-compose up`

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/2ZSNAt?referralCode=97q7Ll)

[How to install the Chrome extension](https://github.com/arc53/docsgpt/wiki#launch-chrome-extension)


## [Guides](https://github.com/arc53/docsgpt/wiki)

## [How to use any other documentation](https://github.com/arc53/docsgpt/wiki/How-to-train-on-other-documentation)

## [How to host it locally (so all data will stay on-premises)](https://github.com/arc53/DocsGPT/wiki/How-to-use-different-LLM's#hosting-everything-locally)

Built with [🦜️🔗 LangChain](https://github.com/hwchase17/langchain)