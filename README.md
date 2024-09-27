


# Character-and-Network-Analysis-in-Text
The project aims to develop an automated model for analyzing the characters and their relationships in books or any type of text documents using statistical and data mining techniques in Python languge programming. The purpose of this automated model is to provide insights into the complex narrative structures and character dynamics found within literary works. 


# Automated Information Extraction Model, Character and Network Analysis in Texts

## Introduction

This project focuses on developing an automated model for analyzing characters and their relationships in literary texts, specifically Jane Austen's "Pride and Prejudice." By utilizing natural language processing (NLP) and information extraction (IE) techniques, the model aims to uncover complex narrative structures and character dynamics within the text. The project involves various stages, including data acquisition, preprocessing, named entity recognition (NER), network analysis, and visualization, ultimately contributing to the field of digital humanities.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Technical Methods](#technical-methods)
- [Results and Conclusions](#results-and-conclusions)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Installation

To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/mo-rahimi/Character-and-Network-Analysis-in-Text

   ```

2. Navigate to the project directory:
   ```bash
   cd yourproject
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the analysis model, execute the following command:
```bash
python main.py
```

This will initiate the automated character and network analysis process on "Pride and Prejudice."

## Technical Methods

The project employs several technical methods, including:

1. **Data Acquisition**: The text of "Pride and Prejudice" is downloaded from Project Gutenberg using the following code snippet:
   ```python
   import requests

   book_id = 1342
   url = f"https://www.gutenberg.org/files/{book_id}/{book_id}-0.txt"
   response = requests.get(url)
   if response.status_code == 200:
       with open("book.txt", "w", encoding="utf-8") as f:
           f.write(response.text)
   ```

2. **Preprocessing**: The text undergoes several cleaning steps, such as removing headers, footers, and special characters, as well as splitting the text into chapters for structured analysis.

3. **Named Entity Recognition (NER)**: A NER pipeline is created using the Hugging Face Transformers library to identify character names within the text.

4. **Network Analysis**: The relationships between characters are analyzed using statistical and data mining techniques, including the creation of co-occurrence matrices and network graphs.

5. **Visualization**: The results are visualized to provide insights into character dynamics and narrative structures.

## Results and Conclusions

The project aims to enhance the understanding of character relationships and narrative structures in literature through automated analysis. By applying the model to "Pride and Prejudice," valuable insights into character dynamics are expected to enrich the reading experience for scholars and literary enthusiasts.

## Contributing

To contribute to this project:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```

3. Make your changes and commit them:
   ```bash
   git commit -m "Add some feature"
   ```

4. Push to the branch:
   ```bash
   git push origin feature-branch
   ```

5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please contact:

- Mohsen Rahimi - [your.email@example.com](mailto:your.email@example.com)
- GitHub: [yourusername](https://github.com/yourusername)

This README provides a comprehensive overview of the project, its objectives, and how to use and contribute to it.

Citations:

[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/24830350/cbf692a7-47e0-46d7-8ef0-caa0ca422a79/Network-Analysis_Report.pdf
