# Marinho Dentistas - Landing Page Interativa

Landing page institucional e de alta conversão para a clínica odontológica de alto padrão **Marinho Dentistas** (@marinho.dentista), situada em Extrema (MG) e Toledo.

---

## 💎 Tecnologias Utilizadas

- **HTML5 Semântico**: Estrutura otimizada para SEO e acessibilidade.
- **Tailwind CSS (via CDN)**: Design system moderno com glassmorphism, paleta noir/dourado suave/caramelo amadeirado e efeitos de luz em LED quente.
- **GSAP & ScrollTrigger (via CDN)**: Sincronização fluida entre a rolagem do usuário e o vídeo institucional de fundo (*Scroll-bound video scrubbing*).
- **Interactive Before/After Image Slider**: Comparador de sorrisos com suporte a eventos de arraste por mouse e toque mobile (*touch*).
- **Integração Direta WhatsApp**: Agendamento rápido com redirecionamento dinâmico.

---

## 📁 Estrutura de Arquivos

```text
MarinhoOdonto/
├── index.html         # Página principal com todo o código integrado
├── vercel.json        # Configuração de headers e range requests para vídeo
├── .gitignore         # Arquivos ignorados pelo Git
├── README.md          # Documentação do projeto
└── assets/
    ├── videos/
    │   └── hero-video.mp4   # Vídeo controlado por ScrollTrigger
    └── images/
        ├── antes.jpg        # Imagem inicial do comparador
        ├── depois.jpg       # Imagem transformada com lentes
        ├── favicon.ico      # Ícone do site
        └── clinic-*.jpg     # Fotos reais da clínica
```

---

## 🚀 Deploy na Vercel

O deploy deste projeto é estático e automatizado através da integração contínua entre **Vercel** e **GitHub**:

1. Ao realizar o `push` para a branch `main` do repositório no GitHub, a Vercel detecta automaticamente os novos commits.
2. A Vercel publica a aplicação instantaneamente em uma URL de produção segura com certificado SSL global e CDN de alta velocidade.
3. O arquivo `vercel.json` garante os cabeçalhos `Accept-Ranges: bytes` e `Cache-Control` ideais para evitar travamentos durante o scrub de vídeo no navegador.
