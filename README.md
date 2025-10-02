# Microsoft AI Avatar – Industry Solutions

This project provides a **web-based AI Avatar interface** built with Azure AI services.  
It integrates with **Azure OpenAI**, **Azure Speech Services**, and **Azure Cosmos DB** to deliver live conversational AI avatars tailored to different industries (Healthcare, Finance, Education, Manufacturing, Retail, etc.).

---

## 🚀 Features

- 🎭 Custom AI Avatars (Binaka, Sri, Mike) with Azure Speech Synthesis
- 💬 Real-time conversational interface (speech-to-text + text-to-speech)
- 🔍 Cognitive Search integration for knowledge mining
- 📊 Session analytics and conversation history
- 🤖 AI-powered recommendations using Azure OpenAI
- 🗄️ Cosmos DB integration for storing sessions and analytics
- 📄 Export consultation reports

---

## 📂 Project Structure

```plaintext
.
├── index.html          # Main web interface
├── css/
│   └── styles.css      # UI styles
├── js/
│   └── chat.js         # Avatar chat logic
├── image/
│   └── attachment.jpg  # Upload icon
└── video/
    └── lisa-casual-sitting-idle.mp4  # Default idle avatar video

AZURE_OPENAI_ENDPOINT=https://<your-resource>.openai.azure.com/
AZURE_OPENAI_API_KEY=<your-key>
AZURE_OPENAI_DEPLOYMENT=gpt-4o

AZURE_SPEECH_KEY=<your-speech-key>
AZURE_SPEECH_REGION=westus2

AZURE_SEARCH_ENDPOINT=https://<your-service>.search.windows.net
AZURE_SEARCH_KEY=<your-key>
AZURE_SEARCH_INDEX=knowledge-base

COSMOS_CONNSTR="mongodb+srv://<username>:<password>@<cosmos-instance>"
COSMOS_DB=customerservice
COSMOS_CONTAINER=AI-Avatar

<input id="azureOpenAIEndpoint" type="text" value="API_ENDPOINT" />
<input id="azureOpenAIApiKey" type="password" value="APIKEY" />
<input id="azureOpenAIDeploymentName" type="text" value="gpt-4o" />

<input id="azureCogSearchEndpoint" type="text" value="SEARCH_ENDPOINT" />
<input id="azureCogSearchApiKey" type="password" value="SEARCH_KEY" />
<input id="azureCogSearchIndexName" type="text" value="INDEX_NAME" />

<!-- Cosmos DB -->
const COSMOS_CONFIG = {
  connectionString: "COSMOSDBSTRING",
  databaseName: "customerservice",
  containerName: "AI-Avatar"
};


git clone https://github.com/<your-org>/ai-avatar-industry.git
cd ai-avatar-industry

Install dependencies (if you extend with Node backend):

npm install


Serve the app locally:

npm start


or open index.html directly in your browser (only works for static demo).

📊 Demo Flow

Select an industry and avatar.

Enter user/company information.

Start the AI Avatar session.

Converse with the avatar (speech or text).

Review analytics and export recommendations.


