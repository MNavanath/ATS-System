# Smart ATS

**Smart ATS** is a web-based application designed to help job seekers enhance their resumes for better performance against Applicant Tracking Systems (ATS). By evaluating resumes against job descriptions in competitive fields like software engineering, data science, and big data engineering, it provides insights on missing keywords, profile summaries, and an ATS compatibility percentage.

The app uses Google’s Generative AI to assess resumes based on a job description, highlighting areas for improvement and optimizing the resume for a specific role. 

## Features

- **Resume Parsing**: Extracts text from uploaded PDF resumes.
- **Generative AI Evaluation**: Uses Google Gemini AI to analyze resumes against job descriptions.
- **ATS Feedback**: Provides percentage matching of resumes to job descriptions, identifies missing keywords, and offers a profile summary.

## Tech Stack

- **Streamlit**: For building the web app interface.
- **Google Generative AI (Gemini)**: For analyzing resumes and job descriptions.
- **PyPDF2**: For extracting text from PDF files.
- **dotenv**: For managing API keys and environment variables.

## Getting Started

### Prerequisites

- **Python 3.7+** installed on your system
- **Streamlit** and other dependencies installed (see below)

### Installation

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/your_username/smart-ats.git
    cd smart-ats
    ```

2. **Install Dependencies**:

    Make sure you have the necessary Python packages installed:

    ```bash
    pip install -r requirements.txt
    ```

3. **Set Up API Key**:

   This project uses Google’s Generative AI (Gemini) for resume evaluation. You will need to get an API key from Google. Once you have the key:

   - Create a `.env` file in the project root:
     
     ```
     touch .env
     ```

   - Add your API key in the `.env` file:
   
     ```
     API_KEY=your_google_gemini_api_key
     ```

4. **Run the Application**:

    Launch the Streamlit app using the following command:

    ```bash
    streamlit run app.py
    ```

    This will start the Smart ATS app in your default browser.

## Usage

1. **Upload Your Resume**: Upload a PDF version of your resume via the file uploader in the web interface.
2. **Enter Job Description**: Paste the job description for the role you're applying to.
3. **Get Feedback**: The app will evaluate your resume and provide insights such as:
   - Matching percentage based on the job description
   - Missing keywords that should be included
   - Profile summary that could help improve your chances

## Project Structure

- `app.py`: The main script that runs the Streamlit app.
- `requirements.txt`: A list of dependencies needed to run the app.
- `.env`: The file that stores your API key (not included in version control).

## Contributing

If you’d like to contribute to the project, feel free to open a pull request. Contributions are welcome in the form of new features, bug fixes, or documentation improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
