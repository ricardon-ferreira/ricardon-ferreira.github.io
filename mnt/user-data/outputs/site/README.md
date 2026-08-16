# ricardon-ferreira.github.io

Site pessoal de Ricardo Nunes Ferreira. Página única, sem build e sem dependências:
todo o HTML e CSS estão em `index.html`.

Endereço final: **https://ricardon-ferreira.github.io**

## Estrutura

```
index.html
IBM/
  publicacoes/
    339-2019-redes-para-containers-en.pdf
    370-2020-o-que-e-python-en.pdf
    387-2021-cloud-distribuida-en.pdf
    394-2021-infraestrutura-para-ai-en.pdf
certificacoes/
  palo-alto/     16 certificados
  wiz/            1 certificado
  kyndryl/        1 certificado
premios/         (aguardando arquivos — ver premios/README.md)
```

### Como adicionar uma certificação

Uma pasta por fabricante, em minúsculas e com hífen: `certificacoes/fortinet/`,
`certificacoes/ibm/`, `certificacoes/microsoft/`. Dentro dela, o arquivo no formato
`AAAA-MM-DD-nome-do-curso.pdf` — a data na frente mantém tudo em ordem cronológica sozinho.

Depois, copie uma linha `<div class="cert">` da seção `#certificacoes` no `index.html`,
troque data, título e caminho. Para um fabricante novo, copie também o `<div class="vend">`
que abre o grupo.


Os PDFs são as versões em inglês, com o certificado de tradução na primeira página.
O Mini Paper Nº 260 (2018) aparece na lista, mas ainda sem link.

## Falta preencher

- `SEU-EMAIL@EXEMPLO.COM` — aparece duas vezes: nos links do topo e no rodapé
- `https://www.linkedin.com/in/SEU-USUARIO` — o endereço real do seu perfil

## Português e inglês

O site é bilíngue. Cada elemento traduzível carrega dois atributos, `data-pt` e
`data-en`, e o botão PT/EN no topo troca o conteúdo sem recarregar a página.
O idioma inicial segue o do navegador do visitante: português para quem tem o
navegador em pt, inglês para todo o resto.

Para editar um texto, altere **os dois** atributos. O texto que aparece escrito
dentro da tag é só o estado inicial — vale manter igual ao `data-pt`.

## Como publicar

1. Crie um repositório público chamado exatamente `ricardon-ferreira.github.io`
2. Em Add file > Upload files, arraste a pasta `site` inteira (não os arquivos soltos,
   ou a estrutura `IBM/publicacoes` se perde)
3. Settings > Pages > Source: "Deploy from a branch", branch `main`, pasta `/ (root)`
4. Um ou dois minutos depois o site responde em https://ricardon-ferreira.github.io

Qualquer edição no `index.html` republica o site sozinha em cerca de um minuto.

## Alterar o conteúdo

- **Linha do tempo:** cada `<div class="ev">` é um evento. A classe `ev--live` marca o
  evento atual em amarelo — deve existir em um bloco só.
- **Publicações:** cada `<div class="pub">` é um artigo.
- **Cores:** todas as cores estão nas variáveis `:root`, no topo do `<style>`.

## Domínio próprio (opcional)

Crie um arquivo `CNAME` na raiz com o domínio dentro (ex.: `ricardoferreira.com.br`),
aponte um registro CNAME no DNS para `ricardon-ferreira.github.io` e ative HTTPS em Settings > Pages.
