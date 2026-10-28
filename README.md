👻 Hollow Hour

Every story leaves something behind.

<p align="center">
  <strong>Where forgotten folklore meets artificial intelligence.</strong>
</p><p align="center">
  <a href="https://hollow-hour.onrender.com/">🌐 Live Demo</a> ·
  <a href="https://github.com/05unique-dotcom/Hollow-Hour">📦 GitHub Repository</a> ·
  <a href="https://github.com/05unique-dotcom/Hollow-Hour/issues">🐛 Report a Bug</a>
</p>---

🌑 About the Project

Hollow Hour is an atmospheric horror storytelling experience inspired by eerie local legends, unexplained encounters, and stories passed down through generations.

Set against the haunting atmosphere of Kudal, Maharashtra, the project explores a simple question:

What happens when the stories we inherit begin answering back?

Hollow Hour combines interactive storytelling, dark visual design, and an AI-powered ghost conversation experience to create a website where visitors can explore unsettling tales and ask questions about the mysteries within them.

Built as a creative web project, Hollow Hour brings together folklore, frontend development, backend integration, and generative AI in one immersive experience.

✨ Features

- 📖 Atmospheric Horror Stories — Explore unsettling tales, including The Old Well, The Voice Under the Peepal, and The Locked Room.
- 👻 Interactive Ghost Chat — Ask questions about the stories and experience an AI-driven conversation inspired by the world of Hollow Hour.
- 🕯️ Immersive Visual Experience — Explore a dark interface with horror-inspired visual effects and an atmospheric presentation.
- 🔦 Torch-Inspired Interactions — Experience lighting effects designed to reinforce the feeling of exploring the unknown.
- 🌘 Gentle Mode & Intro Experience — Enter the experience through an introductory interface with an alternative, gentler presentation.
- 🤖 AI Integration — Connect a language model through the Groq API to generate contextual responses.
- 📱 Browser-Based Experience — Visit the website from a supported mobile or desktop browser without installing a dedicated application.
- 🌐 Online Deployment — Access the project through its publicly hosted website.

«Development note: The AI conversation feature is under active debugging. Responses may be unavailable or incomplete while the backend and model integration are being refined.»

🎮 Experience Hollow Hour

Live website: https://hollow-hour.onrender.com/

1. Open the website in your browser.
2. Enter the Hollow Hour experience.
3. Explore the available horror stories.
4. Ask the ghost questions related to the stories.
5. Discover the atmosphere, clues, and mysteries that make each tale unsettling.

The experience is designed to encourage curiosity while preserving the mystery of the stories.

🛠️ Technology Stack

Technology| Purpose
HTML| Webpage structure
CSS| Styling, atmosphere, and visual effects
JavaScript| Interactive frontend behavior
Node.js| Server-side JavaScript runtime
Express or the server framework configured in the project| HTTP server and request handling
Groq API| AI-generated conversational responses
Render| Web application hosting
Git & GitHub| Version control and collaboration

The exact framework and dependencies should be confirmed against the current project files before treating this table as a definitive architecture specification.

🧩 How It Works

Hollow Hour brings together three main parts:

1. The storytelling interface

The frontend presents the horror stories and interactive elements that visitors use to explore the experience.

2. The application server

The Node.js server handles incoming requests and coordinates communication between the website and the AI service.

3. The AI conversation layer

When a visitor submits a question, the backend sends the relevant prompt to a language model through the Groq API. The response is then returned to the website and displayed in the ghost conversation interface.

Visitor
   │
   ▼
Hollow Hour Web Interface
   │
   ▼
Node.js Server
   │
   ▼
Groq Chat Completions API
   │
   ▼
AI-Generated Response
   │
   ▼
Ghost Conversation Interface

The intended experience is a story-aware conversational interface rather than a generic chatbot. Its response quality depends on the prompt, story context, model availability, and successful API communication.

🚀 Getting Started

Prerequisites

Before running the project locally, make sure you have:

- Node.js installed.
- Git installed.
- A Groq API key for testing the AI conversation feature.
- A modern web browser.

1. Clone the repository

git clone https://github.com/05unique-dotcom/Hollow-Hour.git
cd Hollow-Hour

2. Install dependencies

npm install

3. Configure environment variables

Create a ".env" file in the project root if the application uses "dotenv", or configure the variables through your hosting provider.

GROQ_API_KEY=your_groq_api_key
GROQ_MODEL=openai/gpt-oss-120b
PORT=3000

Important:

- Replace the API key placeholder with your own key.
- Verify that the selected model is currently supported by Groq.
- "GROQ_MODEL" is optional if the server already defines a default model.
- "PORT" is only needed if the server reads it from the environment.
- Never commit real API keys or other secrets to GitHub.

Official references:

- "Groq API Documentation" (https://console.groq.com/docs/api-reference)
- "Groq Text Generation Guide" (https://console.groq.com/docs/text-chat)

4. Start the server

npm start

If the project dependencies and configuration are correct, the server should start according to the configured npm script.

Open the local address printed by the server, or use "http://localhost:3000" if that is the configured port.

«Note: These instructions assume the current project contains a valid "package.json" with a "start" script and the required server files.»

☁️ Deployment

Hollow Hour is hosted on Render.

To deploy your own instance:

1. Fork or clone the repository.
2. Create a new web service in Render.
3. Connect your GitHub repository.
4. Set the build command to "npm install", if required.
5. Set the start command to "npm start".
6. Add the required environment variables through Render's Environment settings.
7. Deploy the service and inspect the logs for startup or API errors.

Keep credentials in environment variables rather than hardcoding them in source files.

Live project: https://hollow-hour.onrender.com/

🔧 Troubleshooting

The ghost is silent

If the website displays a fallback message instead of an AI response:

- Check that "GROQ_API_KEY" is configured correctly.
- Confirm that "GROQ_MODEL" references a supported model.
- Inspect the Render logs for HTTP status codes and API errors.
- Check whether the server receives a valid response containing assistant message content.
- Verify that the frontend correctly handles empty responses and failed requests.

The server cannot find a file

If deployment reports a missing "server.js", HTML file, or another required file:

- Confirm that the file exists in the repository.
- Check filename capitalization and file paths.
- Verify the Render service's root directory and start command.
- Redeploy after committing the necessary changes.

The application starts but returns an empty answer

A successful server startup does not guarantee a successful AI response. Check the API response structure, the model's returned message content, and the server's handling of empty or unexpected results.

🤝 Contributing

Contributions, suggestions, bug reports, and creative ideas are welcome.

If you would like to contribute:

1. Explore the repository and identify an improvement.
2. Open an issue to discuss larger changes.
3. Fork the repository.
4. Create a feature branch.
5. Make a focused change and test it.
6. Submit a pull request explaining what changed and why.

Example:

git checkout -b feature/your-improvement
git add .
git commit -m "feat: describe your improvement"
git push origin feature/your-improvement

For contributions related to AI responses, please include the relevant context and expected behavior without sharing API keys or other sensitive information.

Contribution ideas

- Improve AI responses using story-specific context.
- Add new original horror stories.
- Refine accessibility and mobile responsiveness.
- Improve loading states and error handling.
- Enhance visual effects and performance.
- Add automated tests and documentation.
- Improve the contribution workflow for first-time contributors.

Please ensure that submitted stories and other creative assets are original or appropriately licensed.

🗺️ Roadmap

Potential future improvements include:

- [ ] More original folklore-inspired horror stories.
- [ ] More consistent story-aware AI conversations.
- [ ] Better handling of unavailable models and API failures.
- [ ] Improved mobile accessibility and performance.
- [ ] Automated tests for server routes and response handling.
- [ ] Clearer contribution documentation.
- [ ] Additional atmospheric interactions and storytelling details.

The roadmap is intended to evolve as the project develops.

🔐 Security

- Keep API keys and secrets out of source control.
- Use environment variables for private configuration.
- Never expose server-side credentials to browser JavaScript.
- Report security concerns privately to the project maintainer where possible.

📜 License

Please refer to the repository's ""LICENSE"" (https://github.com/05unique-dotcom/Hollow-Hour/blob/main/LICENSE) file for the applicable license and usage permissions.

👻 A Final Word

Some stories are told to entertain us.

Others are told because someone, somewhere, still remembers what happened.

Hollow Hour — listen closely. The silence may have something to say.

---

<p align="center">
  <sub>Created with curiosity, code, and a fascination with the unexplained.</sub>
</p>
