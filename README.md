# Resume Analyzer with Microsoft Phi-3 Vision-128k-Instruct

This project leverages the Microsoft Phi-3 Vision-128k-Instruct model to analyze resumes and job descriptions, providing actionable recommendations to improve the applicant's chances of securing their desired role.

## Features

- Extracts key information from uploaded resumes (in PDF format):
  - Personal details
  - Educational background
  - Work experience
  - Key skills and proficiencies
  - Notable projects and achievements
- Analyzes job descriptions to identify skill gaps and areas for improvement.
- Provides detailed recommendations for improving resumes and enhancing job compatibility.
- Easy-to-use GUI built with `ipywidgets` for uploading resumes and entering job descriptions.
- Saves analysis results to a text file.

## Installation

### Prerequisites

- Python 3.8 or higher
- `pip` package manager

### Install Required Libraries

Run the following command to install all necessary dependencies:

```bash
pip install transformers PyPDF2 torch ipywidgets
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/resume-analyzer.git
   cd resume-analyzer
   ```

2. Launch the Jupyter Notebook or Jupyter Lab environment:

   ```bash
   jupyter notebook
   ```

3. Open the notebook containing the code (`resume_analyzer.ipynb`) and execute all cells to run the application.

4. Interact with the GUI:
   - Upload a PDF file of your resume.
   - Enter the job description in the text area provided.
   - Click the **Analyze Resume** button to start the analysis.

5. View recommendations and analysis in the output area.

6. Results are automatically saved to `response.txt` for future reference.

## Project Structure

```
resume-analyzer/
├── README.md             # Project documentation
├── requirements.txt      # List of dependencies
├── resume_analyzer.ipynb # Jupyter Notebook with the main code
├── response.txt          # File where analysis results are saved
└── sample_resume.pdf     # Sample resume for testing (optional)
```

## Requirements File

To recreate the environment, install dependencies using the provided `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### Content of `requirements.txt`

```
transformers
PyPDF2
torch
ipywidgets
```

## Notes

- The project uses the Microsoft Phi-3 Vision-128k-Instruct model, which requires GPU for optimal performance. If a GPU is not available, the code will fall back to CPU.
- Ensure you have sufficient permissions to write files to the directory for saving results.


## Acknowledgments

- [Microsoft Phi-3 Vision-128k-Instruct Model](https://huggingface.co/microsoft/Phi-3-vision-128k-instruct)
- [Hugging Face Transformers](https://github.com/huggingface/transformers)

