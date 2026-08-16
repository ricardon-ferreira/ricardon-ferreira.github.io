# ricardonunesferreira.github.io

Site pessoal — página única, sem dependências, sem build. É só HTML e CSS em `index.html`.

## Antes de publicar, edite

- `SEU-EMAIL@EXEMPLO.COM` — aparece em dois lugares (links do topo e rodapé)
- `https://www.linkedin.com/in/SEU-USUARIO`
- `https://github.com/SEU-USUARIO` — ou remova o link, se preferir
- `Winter Garden · Flórida` na barra superior, caso não queira expor a cidade

## Como alterar o conteúdo

- **Linha do tempo:** cada bloco `<div class="ev">` é um evento. Copie um bloco existente para adicionar outro. A classe `ev--live` marca o evento atual em amarelo — deve existir em um bloco só.
- **Publicações:** cada `<div class="pub">` é um artigo.
- **Cores:** todas as cores estão nas variáveis `:root` no topo do `<style>`.

## Estrutura

```
index.html
IBM/
  publicacoes/
    339-2019-redes-para-containers-en.pdf
    370-2020-o-que-e-python-en.pdf
    387-2021-cloud-distribuida-en.pdf
    394-2021-infraestrutura-para-ai-en.pdf
```

Os PDFs são as versões em inglês, com certificado de tradução na primeira página.
Falta o Nº 260 (2018), que continua sem link na página.

## Domínio próprio (opcional)

Crie um arquivo `CNAME` na raiz com o domínio dentro (ex.: `ricardoferreira.com.br`),
aponte um `CNAME` no DNS para `SEU-USUARIO.github.io` e ative HTTPS nas configurações do Pages.
