# Website Food

Landing page estática em HTML, CSS e JavaScript para apresentação de um restaurante/serviço de delivery. O site mostra um herói com chamada para ação, sessão de cardápio, depoimentos e rodapé com redes sociais.

## Visão geral
- **Público-alvo:** equipes que precisam de uma página simples para divulgar um negócio de alimentação e coletar pedidos via botões de contato.
- **Tecnologias:** HTML5, CSS3 e JavaScript vanilla com jQuery e ScrollReveal para interação/animar o scroll, além de ícones do Font Awesome.
- **Arquitetura:** site estático sem backend; todos os arquivos ficam em `index.html` e em `src/` (estilos, imagens e JavaScript). Não há build ou bundler.

## Estrutura do projeto
```
.
├── index.html              # Página principal e único HTML
├── src/
│   ├── images/             # Imagens usadas nos componentes
│   ├── javascript/
│   │   └── script.js       # Lógica de menu mobile, scroll e animações
│   └── styles/
│       ├── styles.css      # Variáveis globais e imports dos demais CSS
│       ├── header.css
│       ├── home.css
│       ├── menu.css
│       ├── testimonials.css
│       └── footer.css
└── .gitignore
```

## Pré-requisitos
- Navegador moderno.
- Opcional: Python 3 (para subir um servidor local simples). Nenhuma dependência extra precisa ser instalada.

## Como rodar localmente (até 10 minutos)
1. Clone o repositório e entre na pasta:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd Website-Food
   ```
2. Abra o arquivo `index.html` diretamente no navegador **ou** sirva os arquivos estáticos com Python para evitar restrições de CORS:
   ```bash
   python -m http.server 8080
   ```
   Depois acesse http://localhost:8080.

## Variáveis de ambiente
- O projeto não utiliza variáveis de ambiente.

## Comandos úteis
- Servir o site localmente (porta 8080):
  ```bash
  python -m http.server 8080
  ```

## Frontend
- Layout responsivo com breakpoints em 1170px e 600px para menu mobile, CTA e depoimentos.
- Botão de menu mobile alterna visibilidade e ícone via jQuery.
- Destaques animados com ScrollReveal em CTA, pratos e depoimentos.

## Deploy
Por ser um site estático, você pode publicar o conteúdo deste repositório em serviços como GitHub Pages, Netlify ou qualquer hospedagem que aceite arquivos estáticos. Basta apontar a raiz do site para a pasta do projeto (onde está `index.html`).
