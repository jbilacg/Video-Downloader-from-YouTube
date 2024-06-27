import os
import random
import string
from pytube import YouTube

# Lista de links do YouTube para download
links = [
    "https://www.youtube.com/watch?v=l4rmTpnT3Jg",
    "https://www.youtube.com/watch?v=TXmtmmGb-zk",
    "https://www.youtube.com/watch?v=LJwdn8CuXwI",
    "https://www.youtube.com/watch?v=BcgetZmzHIg",
    "https://www.youtube.com/watch?v=Wi-wSgmi3C4",
    "https://www.youtube.com/watch?v=nRnVPmPJeQE"
]

# Gera um nome aleatório para a pasta de download
random_folder_name = ''.join(random.choices(string.ascii_lowercase + string.digits, k=8))

# Diretório de download
download_dir = r"C:\Users\Jess\Downloads\vídeos EJA\EJApt1"

# Itera sobre a lista de links para baixar os vídeos
for link in links:
    try:
        youtube = YouTube(link)
        video = youtube.streams.get_highest_resolution()
        video.download(output_path=download_dir)
        print(f"Downloaded: {youtube.title}")
    except Exception as e:
        print(f"Error downloading {link}: {str(e)}")
