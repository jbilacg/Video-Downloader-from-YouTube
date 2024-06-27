# Video Downloader from YouTube

Este projeto em Python baixa vídeos do YouTube a partir de uma lista de links e os salva em uma pasta específica. Utiliza a biblioteca `pytube` para interagir com o YouTube.

## Requisitos

- Python 3.x
- Biblioteca `pytube`

Você pode instalar a biblioteca `pytube` usando o seguinte comando:

```sh
pip install pytube

## Explicação do Script
O script downloader.py realiza as seguintes etapas:

### Importações:

- os: Módulo para interagir com o sistema operacional.
random e string: Módulos para gerar nomes de pastas aleatórios.
pytube: Biblioteca para baixar vídeos do YouTube.
Lista de links:

- Uma lista de URLs de vídeos do YouTube a serem baixados.
Geração de nome aleatório para a pasta:

- Usa random.choices para criar um nome de pasta aleatório com letras minúsculas e dígitos.
Diretório de download:

- O caminho onde os vídeos baixados serão salvos.

## Iteração e download:

Para cada link na lista:
Tenta criar um objeto YouTube com o link.
Obtém o stream de vídeo com a mais alta resolução.
Baixa o vídeo para o diretório especificado.
Imprime uma mensagem de sucesso.
Se ocorrer um erro, uma mensagem de erro será impressa.
Contribuição
Se você quiser contribuir para este projeto, por favor siga os passos abaixo:

Faça um fork do repositório.
Crie uma nova branch: git checkout -b minha-feature
Faça suas alterações e commite: git commit -m 'Minha nova feature'
Envie para a branch original: git push origin minha-feature
Crie um pull request.
