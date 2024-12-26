# Teams Chat Export Tool

A JavaScript tool to export Microsoft Teams chat messages into a Markdown file. This script helps you save and archive your Teams conversations, complete with messages, timestamps, sender information, and images.

## Features

- **Export Chats to Markdown**: Converts your Teams chat history into a neatly formatted Markdown file.
- **User-Friendly Interface**: Provides a control panel with options to adjust scroll delay, stop the export process, preview the Markdown output, and toggle between light and dark themes.
- **Image Support**: Captures images shared in the chat and includes them in the export.
- **Customizable Output**: Allows you to set custom chat titles and filenames for your exports.

## Getting Started

### Prerequisites

- Access to [Microsoft Teams Web Client](https://teams.microsoft.com/)
- A modern web browser (e.g., Chrome, Firefox, Edge)

### How to Use

1. **Navigate to Microsoft Teams Web**:
   - Open your web browser and go to [teams.microsoft.com](https://teams.microsoft.com/).
   - Log in with your Microsoft account if you aren't already logged in.

2. **Open the Chat to Export**:
   - Navigate to the specific chat or channel you want to export.

3. **Access Developer Console**:
   - Press `F12` or right-click the page and select **Inspect** to open the developer console.

4. **Paste and Run the Script**:
   - Copy the entire script from the `exportTeamsChat()` function in this repository.
   - Paste it into the console and press `Enter`.

5. **Start the Export Process**:
   - In the console, type `exportTeamsChat();` and press `Enter`.
   - A new window will open with the export interface.

6. **Configure Export Settings**:
   - **Chat Title**: Edit the chat title if needed.
   - **Export Filename**: Set your preferred filename for the Markdown file.
   - **Scroll Delay**: Adjust the scroll delay if the default doesn't work well for your chat size.

7. **Begin Export**:
   - The script will scroll through the chat, collecting messages. You can monitor the progress in the new window.

8. **Download the Export**:
   - Once the export is complete, click the **"Download as Markdown"** button to save the chat history to your local machine.

9. **Preview and Adjust**:
   - Use the Markdown preview in the export window to review the output.
   - Toggle between light and dark themes or show/hide the preview.

## Notes

- **Pop-up Blockers**: Ensure your browser allows pop-ups from `teams.microsoft.com`, as the script opens a new window for the export interface.
- **Performance**: For large chats, you might need to adjust the scroll delay or be patient as the script collects all messages.
- **Privacy**: Be cautious when exporting chats that contain sensitive information. Ensure compliance with your organization's data handling policies.

## Troubleshooting

- **Script Not Running**: Make sure you're on the Microsoft Teams web client and have correctly pasted the entire script into the console.
- **No Messages Found**: Verify that you've clicked on the chat area before running the script to ensure the DOM elements are loaded.
- **Export Stops Early**: Try increasing the `noNewMessagesThreshold` or `delayTime` in the configuration if the export doesn't capture all messages.

## Acknowledgments

- **Original Script by [blaze_125](https://stackoverflow.com/users/5884037/blaze-125)**:
  - This tool is based on the script provided by [blaze_125](https://stackoverflow.com/a/77558238/11682706) on Stack Overflow.
  - Special thanks for the initial development and sharing of the script, which has been adapted and expanded upon in this project.

## Contributing

Feel free to submit issues or pull requests to improve this tool. Contributions are welcome!

## License

This project is licensed under the [MIT License](LICENSE).

## Disclaimer

This tool is provided as-is and is not affiliated with Microsoft. Use it at your own risk, and ensure you comply with Microsoft's terms of service and your organization's policies when exporting chat data.
