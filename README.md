Look through law files in GEMINI-TEST-Folder and see if they follow the principle of contra proferentum (using Google Gemini). 

Before inputting the files for analysis by the LLM, you must check to see if they have been extracted correctly by the PDF Reader (ex. print their output)
For example, 1.pdf does not have much selectable text and was not being read correctly, so it needed to use OCR (ex. via smallpdf.com, which would convert the original pdf file
into a pdf with searchable text)
    -- other PDF readers could have been used, like pdf2image and tesseract (the code of which has been commented out since it takes around ~10 minutes for the text extraction to finish;
    the commented out portion of the code will still work (it just takes longer)---the only change will be to replace 1o.pdf with 1.pdf in the analysis and to comment out the part of the code in the same cell that uses pdfreader)

DEPENDENCIES:
pip install PyPDF2
pip install google-generativeai
pip install python-dotenv
----- and, if want to use pdf2image and tesseract instead: pip install pdf2image, pip install pytesseract

NOTE: You must create a .env file with the following:
    GENAI_API_KEY = YOUR_API_KEY