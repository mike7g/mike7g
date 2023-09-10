- 👋 Hi, I’m @mike7g
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mike7g/mike7g is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
!pip install git+https://github.com/openai/whisper.git -q
!pip install pytube -q
import whisper
from pytube import YouTube
model = whisper.load_model('base')
youtube_video = YouTube("https://www.youtube.com/watch?v=Jv71pCKqT3c")
print(youtube_video.title)
for stream in youtube_video.streams:
  print(stream)
