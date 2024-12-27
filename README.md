Look through law files in GEMINI-TEST-Folder and see if they follow the principle of contra proferentum (using Google Gemini). 

Before inputting the files for analysis by the LLM, you must check to see if they have been extracted correctly by the PDF Reader (ex. print their output)
For example, 1.pdf does not have much selectable text and was not being read correctly, so it needed to use OCR (ex. via smallpdf.com, which would convert the original pdf file
into a pdf with searchable text)
    -- other PDF readers could have been used, like pdf2image and tesseract (the code of which has been commented out), but these were still not working well (majority of pdf text was still not being read properly)

DEPENDENCIES:
pip install PyPDF2
pip install google-generativeai
pip install python-dotenv

NOTE: You must create a .env file with the following:
    GENAI_API_KEY = YOUR_API_KEY