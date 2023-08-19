how to compile:
1. clone git repo
2.  docker container and mount volume:
```
docker run -it -v /home/config/code/bitcoinbook:/documents/ asciidoctor/docker-asciidoctor
```
3. Compile:
- pdf:
  ```
  asciidoctor-pdf -r asciidoctor-mathematical -d book -a pdf-theme=custom_themes/basic.yml book.asciidoc
  ```
- epub:
  ```
  asciidoctor-epub3 -r asciidoctor-mathematical -d book -a pdf-theme=custom_themes/basic.yml book.asciidoc
  ```




