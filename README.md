###MyPilot VSCode Extension
Overview
The MyPilot extension for Visual Studio Code is an AI-powered coding assistant designed to enhance the coding experience by providing contextual help and code suggestions. This extension integrates with an AI model to assist users with their coding queries based on the surrounding code context.
Features
Contextual Code Assistance: The extension captures surrounding lines of code and allows users to ask questions about the code context.
Webview Interface: A user-friendly chat interface where users can interact with the AI assistant.
Error Handling: Comprehensive error handling to manage API request failures and inform users appropriately.
Installation
Clone the Repository: Clone this repository to your local machine.
Open VSCode: Launch Visual Studio Code and open the cloned folder.
Install Dependencies: Run npm install to install the necessary dependencies.
Run the Extension: Press F5 to start debugging the extension in a new VSCode window.
Usage
Open the Chat: Use the command palette (Ctrl+Shift+P) and type Open Chat to open the MyPilot chat interface.
Ask Questions: Type your coding question in the chat box and press send. The AI will respond based on the surrounding code context.
Error Messages: If there are issues with the API or other errors, the extension will display an appropriate message.
Code Structure
extension.ts: The main file containing the logic for the extension, including AI querying and handling user interactions.
AI Integration: Utilizes Axios for making API calls to the AI service, with error handling for network issues.
Example Code Snippet
typescript
async function queryAIWithContext(surroundingText: string, userQuery: string): Promise<string> {
    const prompt = `### Code Context ###\n${surroundingText}\n\n### User's Question ###\n${userQuery}`;
    // API call logic...
}

Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments
Thanks to the developers of the AI model and the VSCode API for making this extension possible.

Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments
Thanks to the developers of the AI model and the VSCode API for making this extension possible.
