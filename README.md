# Navart Entretenimento

Site institucional da Navart Entretenimento, de Sorocaba (SP): personagens vivos,
caracterizacao e atracoes para eventos, ativacoes de marca e datas comemorativas.

Producao: ASKN.

## Como e feito

Pagina unica, sem dependencias e sem etapa de build. Tudo vive em `index.html`:
marcacao, estilo e comportamento. As fotos ficam em `img/`.

Para ver localmente, basta abrir `index.html` no navegador. Nao precisa de servidor.

## Publicacao

A previa publica sai do GitHub Pages, servida do ramo `main`, pasta raiz.
O arquivo `.nojekyll` desliga o processamento Jekyll, que nao e usado aqui.

`robots.txt` bloqueia a indexacao enquanto isto e uma previa. Ao migrar para o
dominio definitivo, troque o conteudo por `Allow: /` para liberar as buscas.

## Dominio proprio

Para apontar um dominio registrado no Registro.br:

1. No repositorio, crie um arquivo `CNAME` com o dominio, por exemplo `navart.com.br`.
2. No painel do Registro.br, em DNS, aponte os registros `A` do dominio raiz para
   `185.199.108.153`, `185.199.109.153`, `185.199.110.153` e `185.199.111.153`.
3. Crie um `CNAME` para `www` apontando para `thiglimaASKN.github.io`.
4. Em Settings, Pages, informe o dominio e marque **Enforce HTTPS** assim que o
   certificado for emitido.
