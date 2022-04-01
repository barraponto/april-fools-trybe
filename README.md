<div align='center'>
  <hr />
  <br />
  <h1>Trybe April Fools</h1>
  <p>É isso que acontece quando uma pessoa tem muito tempo livre.</p>
  <br />
  <hr />
</div>

## Como?

Então, não tinha vulnerábilidade na Trybe, mas usei uma técnica chamada <a href="https://pt.wikipedia.org/wiki/Clickjacking" target="_blank" rel="noopener noreferrer">clickjacking</a> pra explorar a ferramenta do markdown (formatação de texto) do Slack de forma a mostrar um link confiável e ao clicar enviar o usuário para um outro, nesse caso, um <a href="https://www.techtudo.com.br/noticias/2017/11/ataque-homografico-truque-na-url-engana-usuarios-com-paginas-falsas.ghtml" target="_blank" rel="noopener noreferrer">lookalike domain</a>, um domínio que se parece muito com outro confiável à primeira vista.

![](https://user-images.githubusercontent.com/61599784/161175933-a259c1ee-4327-4eb7-a78c-2c4f6eb1c2f0.png)

Nesse caso o url exibido é o da Trybe de verdade seguido por coisas sem sentido nenhum, porém aqui ele age como um texto para o link, que por sua vez termina com ptr.red, um domínio ao qual tenho controle.

```
https://www.betrybe.com/r/[...]
https://www.betrybe.com.ptr.red/r/[...]
```

Crei uma tela de loading para criar expectativa e nela usei a fonte, as cores e o logo da Trybe para parecer oficial. Após 1,5 segundos o úsuario é redirecionado para um <a href="https://support.google.com/youtube/answer/171780?hl=pt-BR" target="_blank" rel="noopener noreferrer">link embed do YouTube</a> que reproduz automáticamente <a href="https://ptr.red/trr" target="_blank" rel="noopener noreferrer">o melhor vídeo da internet</a>.

## Por que?

Sei lá, normalmente todo ano planejo algo desnecessáriamente complicado pro primeiro de abril e como é minha segunda semana na Trybe e estou muito empolgado com tudo, decidi fazer isso, espero muito não ser expulso.

## O que podemos aprender com isso?

Nada, foi uma ideia idiota e quanto mais tempo eu passo nisso menos graça parece ter, mas agora já fui longe demais pra voltar então se quiser tirar um valor educacional ou instrutivo disso, que esse seja **sempre esteja atento aos links que clica e/ou navega**, porquê essas técnicas são usadas por milhares de _scammers_ todo dia e contribuem para a aplicação de <a href="https://pt.wikipedia.org/wiki/Phishing" target="_blank" rel="noopener noreferrer"><i>phishing</i></a>, diversos tipos de golpes e infecções por _malwares_.

## Tecnologias

O framework usado foi o <a href="https://nextjs.org/" target="_blank" rel="noopener noreferrer">NextJS</a> (através do <a href="https://nextjs.org/docs/api-reference/create-next-app" target="_blank" rel="noopener noreferrer">create-next-app</a>), só porque amo ele e é o que eu mais tenho familiaridade. Como fiz esse projeto na noite do dia 31 e só tinha aproximadamente 2 horas, usei também o <a href="https://tailwindcss.com/" target="_blank" rel="noopener noreferrer">TailwindCSS</a> para estilizar a página do jeito mais rápido possível. <a href="https://yarnpkg.com/" target="_blank" rel="noopener noreferrer">Yarn</a> é o gerenciador de pacotes, o site foi hospedado na <a href="https://vercel.com/" target="_blank" rel="noopener noreferrer">Vercel</a> e a trilha sonora é cortesia de <a href="https://pt.wikipedia.org/wiki/Rick_Astley" target="_blank" rel="noopener noreferrer">Richard Paul Astley</a>.

## Jabá e informações adicionais

Se você assim como eu acha que eu levei essa piada longe demais e perdi muito tempo, me segue no <a href="https://ptr.red/gh" target="_blank" rel="noopener noreferrer">GitHub</a> porque eu faço isso mais do que eu gostaria de admitir.

Se quiser saber mais ou tiver dúvidas sobre isso ou qualquer outra coisa, para entrar em contato comigo <a href="https://ptr.red/contact-me" target="_blank" rel="noopener noreferrer">clique aqui</a> ou me mande uma mensagem direta no Slack. #VQV 💚

<div align="center">
  <br />
  <a href="https://ptr.red/tt" target="_blank" rel="noopener noreferrer">
    <img alt="Twitter" src="https://img.shields.io/badge/TWITTER-1DA1F2?style=for-the-badge&logo=twitter&logoColor=FFFFFF" />
  </a>
  <a href="https://ptr.red/ig" target="_blank" rel="noopener noreferrer">
    <img alt="Instagram" src="https://img.shields.io/badge/INSTAGRAM-E4405F?style=for-the-badge&logo=instagram&logoColor=FFFFFF" />
  </a>
  <a href="https://ptr.red/kb" target="_blank" rel="noopener noreferrer">
    <img alt="Keybase" src="https://img.shields.io/badge/KEYBASE-33A0FF?style=for-the-badge&logo=keybase&logoColor=FFFFFF" />
  </a>
  <a href="mailto:me@peterfritz.dev" target="_blank" rel="noopener noreferrer">
    <img alt="E-mail" src="https://img.shields.io/badge/EMAIL-EA4335?style=for-the-badge&logo=gmail&logoColor=FFFFFF" />
  </a>
  <a href="https://ptr.red/tg" target="_blank" rel="noopener noreferrer">
    <img alt="Telegram" src="https://img.shields.io/badge/TELEGRAM-26A5E4?style=for-the-badge&logo=telegram&logoColor=FFFFFF" />
  </a>
  <a href="https://ptr.red/in" target="_blank" rel="noopener noreferrer">
    <img alt="LinkedIn" src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=FFFFFF" />
  </a>
</div>
