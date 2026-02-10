# examtopics
```
docker run -it \
  --name examtopics-downloader \
  --platform linux/arm64 \
  ghcr.io/thatonecodes/examtopics-downloader:latest \
  -p microsoft -s pl-600 \
  -o pl-600.md -type pdf
docker cp examtopics-downloader:/app/pl-600.md .
docker cp examtopics-downloader:/app/pl-600.pdf .
docker rm examtopics-downloader
```
