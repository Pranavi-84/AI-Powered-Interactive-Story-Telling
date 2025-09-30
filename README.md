# AI-Powered-Interactive-Tale-Narration
An AI-powered storytelling tool for children that generates a story from a letter or image, creates illustrations via Stable Diffusion, produces audio in English, Tamil, and French, and generates an animated video using Pika Labs. It provides an interactive, multilingual learning experience.

INPUT :
A letter of the alphabet (e.g., "A"), or an image (AI describes it).

The system then:
✅ Writes a story (Google Gemini)
✅ Creates an illustration (Stable Diffusion)
✅ Narrates in English, Tamil, and French (gTTS)
✅ Produces a video with image + narration (MoviePy)

FEATURES :

Story generation (letter or image → story).

AI illustration prompt generation.

Stable Diffusion-based image creation.

Multilingual narration (EN, TA, FR).

Automatic video creation.

INSTALLATION :

Clone this repository:

git clone https://github.com/Pranavi-84/AI-Powered-Interactive-Story-Telling.git
cd AI-Powered-Interactive-Story-Telling

PROCESS :
1.Create a virtual environment (recommended):
    python -m venv venv
    source venv/bin/activate    # macOS/Linux
    venv\Scripts\activate       # Windows

2.Install dependencies:

  pip install -r requirements.txt

3.Environment Setup

  3.1Set your API keys:

  Linux/macOS:
    export API_KEY="your_google_genai_api_key"
    export HUGGINGFACE_TOKEN="your_huggingface_token"


  Windows (PowerShell):
    $env:API_KEY="your_google_genai_api_key"
    $env:HUGGINGFACE_TOKEN="your_huggingface_token"

4. Usage

    Run the script:
       python main.py


5.Choose input type:

  Letter mode (L): Generates story, illustration, narration, and video.
    
  Image mode (I): Generates story, narration, and video.

6.Output

  Story → printed in console.
    
  Image → <LETTER>_story_image.png
    
  Audio files → <PREFIX>story_audio[en|ta|fr].mp3
    
  Video → <PREFIX>_story_video.mp4


 EXAMPLE

Input: Letter B

Story: “Bunny bakes bread...”

Image: Bunny baking bread illustration (AI generated)

Audio: Narration in English, Tamil, French

Video: Story image + English narration
