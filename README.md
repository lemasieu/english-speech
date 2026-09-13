# English Speech

A simple, interactive web tool that converts between English text and its IPA (International Phonetic Alphabet) transcription. It supports both American English and British English pronunciations.

## 🚀 Live Demo

Check out the live demo: [https://www.xn--msiu-goa8b.vn/github/english-speech](https://www.xn--msiu-goa8b.vn/github/english-speech)

## ✨ Features

- **English to IPA** – Convert English words and sentences into their IPA phonetic transcription
- **American & British English** – Choose between American English and British English pronunciation
- **Word-by-Word Conversion** – Each word is transcribed individually for accurate results
- **Real-Time Results** – View the IPA transcription instantly after clicking the convert button
- **Clean Interface** – Minimal, user-friendly design with a clear layout
- **Responsive** – Works on desktop, tablet, and mobile devices

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- JSON (IPA dictionary data)
- Python (data generation script)

## 📁 Project Structure

```
english-speech/
├── index.html            # Main HTML file
├── style.css             # Stylesheet
├── script.js             # JavaScript conversion logic
├── ipa_dictionary.json   # IPA dictionary data (based on CMUdict)
├── ipa.py                # Python script for generating the IPA dictionary
└── README.md             # Project documentation
```

## 🔧 Installation & Usage

1. **Clone the repository**
   ```bash
   git clone https://github.com/lemasieu/english-speech.git
   ```
2. **Navigate to the project folder**
   ```bash
   cd english-speech
   ```
   
3. **Run the application with a local server**

⚠️ Important: This project loads data from a JSON file, so you need to use a local development server instead of opening `index.html` directly in your browser to avoid CORS issues.

- **Using VS Code** – Install the "Live Server" extension, right-click on `index.html`, and select "Open with Live Server"
- **Using Python** – Run `python -m http.server` (Python 3) or `python -m SimpleHTTPServer` (Python 2) and open `http://localhost:8000`
- **Using Node.js** – Install `http-server` globally (`npm install -g http-server`) and run `http-server` in the project folder

## 📝 How It Works

1. **Enter English text** – Type or paste any English word or sentence into the input field
2. **Select the accent** – Choose between Tiếng Anh (Mỹ) (American English) and Tiếng Anh (Anh) (British English)
3. **Click "Chuyển đổi" (Convert)** – The tool processes the text and generates the IPA transcription
4. **View the result** – The IPA transcription appears in the output field, word by word

**How the conversion works:**

The tool looks up each word in the `ipa_dictionary.json` file, which is based on [CMUdict](http://www.speech.cs.cmu.edu/cgi-bin/cmudict) (Carnegie Mellon University Pronouncing Dictionary). Each word is matched to its corresponding IPA transcription for the selected accent.

The `ipa.py` Python script is included for generating or updating the IPA dictionary data from the CMUdict source.

**Supported Input:**

- Single words (e.g., `hello`)
- Full sentences (e.g., `Hello, how are you?`)
- Both lowercase and uppercase text

## 🤝 Contributing

Contributions are welcome! Feel free to submit a Pull Request or open an Issue.
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open-source and available under the MIT License.
