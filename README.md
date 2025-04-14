Here's the `README.md` file in the markdown format:

```markdown
# AI-Powered YouTube Comment Sentiment & Toxicity Analyzer

This project leverages **Hugging Face Transformers**, **unitary/toxic-bert**, and **Gradio** to create an AI-powered tool that analyzes the sentiment and toxicity of YouTube comments. The app fetches YouTube comments, analyzes their sentiment (positive or negative) and toxicity (toxic vs. non-toxic), and visualizes the results in an interactive format. It also allows you to filter comments by sentiment or toxicity and download the results as a CSV file.

## Key Features:
- **Sentiment Analysis**: Detects the sentiment of comments (positive/negative).
- **Toxicity Detection**: Uses a pre-trained model to detect different types of toxicity (e.g., toxicity, severe toxicity, identity attack, etc.).
- **Filters**: Filter results based on sentiment and toxicity.
- **Interactive Visualization**: Plot the sentiment distribution using Plotly.
- **Downloadable Results**: Export the analysis results as a CSV file.

## Project Setup

### Requirements:
To run this project locally, you'll need the following dependencies:
- Python 3.7+
- `gradio`
- `transformers`
- `google-api-python-client`
- `plotly`
- `pandas`

You can install these dependencies using `pip`:

```bash
pip install gradio transformers google-api-python-client plotly pandas
```

### YouTube API Key:
You need a **YouTube Data API v3** key to fetch YouTube comments. You can get the API key from the Google Developer Console.

1. Go to [Google Developer Console](https://console.developers.google.com/).
2. Create a project.
3. Enable the **YouTube Data API v3**.
4. Create credentials to get your API key.
5. Replace the `YOUTUBE_API_KEY` variable in the `app.py` file with your own key.

### Running the App:
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/youtube-comment-sentiment-analyzer.git
   cd youtube-comment-sentiment-analyzer
   ```

2. Run the app:
   ```bash
   python app.py
   ```

   This will launch a Gradio interface in your browser, where you can input a YouTube video URL and analyze the comments.

## Usage

1. **Input**: Paste a YouTube video URL into the "YouTube Video URL" textbox.
2. **Settings**:
   - **Number of Comments**: Set the maximum number of comments to fetch (1-100).
   - **Filter by Sentiment**: Choose between **POSITIVE**, **NEGATIVE**, or **All**.
   - **Filter by Toxicity**: Choose the level of toxicity (e.g., **toxicity**, **severe_toxicity**, **Not Toxic**, etc.).
3. **Output**:
   - **Analysis Table**: Displays the sentiment and toxicity analysis of the comments.
   - **Sentiment Distribution Plot**: Visualizes the sentiment distribution of comments.
   - **Download CSV**: Allows you to download the results as a CSV file.

## Example

1. Open the app and paste a YouTube URL (e.g., a music video).
2. Set the number of comments to 50.
3. Choose your desired filters (e.g., **All** sentiments, **Not Toxic**).
4. Click **Analyze Comments**.
5. View the table and sentiment distribution chart.
6. Download the results as a CSV file.

## Contribution

Feel free to fork this repository, make improvements, or open an issue if you encounter any bugs. Contributions are welcome!

### Bug Reports
If you encounter any bugs or issues with the app, please report them through the [Issues](https://github.com/yourusername/youtube-comment-sentiment-analyzer/issues) section.

### Improvements
You can contribute by:
- Adding support for more languages in sentiment analysis.
- Enhancing toxicity detection by training additional models.
- Improving the visualization with more interactive charts.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

Make sure to replace the placeholder text such as `https://github.com/yourusername/youtube-comment-sentiment-analyzer.git` with the actual link to your repository.
