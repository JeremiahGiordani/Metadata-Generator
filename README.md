# Metadata-Generator

This project helps you generate a title, description, and 50 keywords for your stock video files. The system automatically analyzes your uploaded videos to provide the best metadata for describing your videos on stock footage platforms.

You can run it by following the directions below, or going to the publically available <a href='https://colab.research.google.com/drive/1SOC2HraepTh0ifOzvhZseWnx72U22qB0?usp=sharing'>Google Colab notebook<a>

## Features
- Automatically generates video titles, descriptions, and keywords using OpenAI's GPT API.
- Supports processing of multiple `.mp4` and `.mov` video files.
- Outputs results both in the notebook and as a pipe-delimited text file (`video_metadata_output.txt`).

---

## Google Colab Instructions

This platform helps you generate a title, description, and 50 keywords for your stock video files. Simply upload your videos, and the system will handle the rest!

### How to Use:
1. Open the provided notebook in Google Colab.
2. In the code cell where prompted, paste your OpenAI API key inside the quotes.
3. Click on the "File" icon on the left panel to upload your video files. (This might take a little while, so be sure to wait until the videos are completely uploaded.)
4. Once the files are uploaded, click the "Runtime" tab and select "Run All" to start processing.
5. Scroll down to the output. You will see a checklist of the available video files. Select the videos you wish to process by checking the corresponding boxes.
6. Once you have made your selections, click the "Generate" button to start the analysis.
7. After the analysis is complete, the output will show the video title, description, and 50 keywords.
8. You can copy the title, description, and keywords from the output for your use.
9. To view and download the output file, click on the "Files" icon on the left panel. If you don't see the file immediately, refresh the file list. Once you locate the output file (`video_metadata_output.txt`), you can click on it to download and save it to your local machine.

---

## Local Instructions

If you want to run this project locally on your own machine, follow the instructions below.

### Prerequisites:
- Python 3.x
- OpenAI API key (needed to generate video metadata)

### How to Install and Run Locally:
1. **Clone the repository**:
   ```bash
   git clone https://github.com/JeremiahGiordani/Metadata-Generator
   cd stock-video-metadata-generator
   ```

2. **Install the required packages**:
   Install the necessary dependencies using the `requirements.txt` file.
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your OpenAI API key**:
   Create an environment variable to store your OpenAI API key. In your terminal, run:
   ```bash
   export OPENAI_API_KEY='your-api-key-here'
   ```

   Alternatively, modify the code in the notebook to prompt you for the API key.

4. **Prepare your video files**:
   Place your `.mp4` video files inside the `Test Media` folder or any accessible folder.

5. **Run the notebook**:
   You can open the notebook (`MetaDataGenerator (release 1-0-0).ipynb`) in Jupyter Notebook or JupyterLab and run it.

6. **Processing videos**:
   The notebook will automatically find and process all `.mp4` files in the directory, generating titles, descriptions, and keywords for each video.

7. **View the output**:
   The results (title, description, keywords) will be displayed in the notebook and saved to the file `video_metadata_output.txt`.

### Notes:
- If you want to add new videos, place them in the appropriate folder and rerun the notebook.
- Ensure your OpenAI API key is kept secure, and don't share it publicly.

