[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vgbm4cZ0)

Simple-to-use, AI-assisted application that scans corporate documents for compliance with ADGM (Abu Dhabi Global Market) rules through Streamlit and the Google Gemini API.

Launch the App:

You don't have to install anything — just click to launch the app in your browser:
[Launch the App](https://agenthuman-dqnpypanywyr6am9z9dcpa.streamlit.app/)

What It Does:

- Upload `.docx`, `.pdf`, or `.txt` files such as UBO Declarations and Memorandum of Association.
- AI flags compliance issues, categorized by severity: High, Medium, or Review.
- Easy-to-understand suggestions let you easily resolve issues (e.g., add the particular nationality or adhere to ADGM laws).
- See results in a clean table — no frills, no mess.

How It Works:

1. You upload documents via the Streamlit-friendly UI.
2. The app pulls out text (supported by `.docx`, `.pdf`).
3. Google Gemini AI checks the content against ADGM reference materials.
4. You receive a structured list of results with severity, snippets, and recommendations.
5. Optionally save a JSON report or annotated copies of your documents.

To Run It Locally:

(bash)
1. Clone the repo
git clone https://github.com/YOUR-USERNAME/ai-engineer-task-LishigaT.git
cd ai-engineer-task-LishigaT

2. Install the requirements
pip install -r requirements.txt

3. Put your Gemini API key (don't commit this!)
mkdir -p .streamlit
echo 'GEMINI_API_KEY="your_api_key_here"' > .streamlit/secrets.toml

4. Run the app
streamlit run app.py
