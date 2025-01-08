# Customized WhatsApp Chat Suggestion

## Overview
"Customized WhatsApp Chat Suggestion" is an AI/ML-based project designed to enhance your WhatsApp chatting experience by providing personalized word suggestions. The system learns from the user's past chats to offer tailored suggestions, making communication faster and more efficient.

## Features
- **Personalized Suggestions:** The model provides word suggestions based on individual chat history.
- **AI/ML Integration:** Uses Natural Language Processing (NLP) techniques to analyze and predict text.
- **Customizable Training Data:** Users can provide their exported WhatsApp chats as input to the model.

## Requirements
- Python 3.7+
- Required Libraries:
  - pandas
  - numpy
  - scikit-learn
  - tensorflow/keras
  - nltk

## How It Works
1. **Chat Export:** The user exports their WhatsApp chat as a `.txt` file.
2. **Data Preprocessing:**
   - The exported chat file is cleaned and structured for analysis.
   - NLP techniques are applied to tokenize and process the text.
3. **Model Training:**
   - A machine learning model is trained on the processed chat data.
   - The model learns patterns and frequently used words/phrases.
4. **Prediction:**
   - Based on the current input text, the model predicts and suggests the next word or phrase.

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository/customized-whatsapp-chat-suggestion.git
   cd customized-whatsapp-chat-suggestion
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Export your WhatsApp chat:
   - Open a chat in WhatsApp.
   - Tap on the menu (three dots) > "More" > "Export Chat."
   - Save the exported `.txt` file.
4. Place the exported `.txt` file in the `data/` directory.
5. Run the preprocessing script:
   ```bash
   python preprocess_chat.py --input data/your_chat.txt --output data/processed_chat.csv
   ```
6. Train the model:
   ```bash
   python train_model.py --data data/processed_chat.csv
   ```
7. Start the suggestion system:
   ```bash
   python suggest.py
   ```

## Usage
- After running `suggest.py`, input a sentence fragment.
- The system will output personalized word suggestions based on your chat history.

## Future Enhancements
- Support for multiple chat formats.
- Integration with messaging platforms for real-time suggestions.
- Enhanced prediction accuracy using advanced models like GPT.

## Contributing
Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- Inspired by the need for personalized AI solutions in everyday communication.
- Thanks to the open-source NLP and ML communities for their tools and libraries.

