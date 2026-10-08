# Lume Eventos — Site institucional em WordPress

Projeto de portfólio: website profissional para uma produtora de eventos **fictícia**, desenvolvido como se fosse uma demanda real de cliente, do briefing à publicação.

> **Aviso:** a Lume Eventos, seus eventos, clientes e depoimentos são **fictícios** e existem apenas para fins de estudo e portfólio. Imagens de terceiros pertencem aos respectivos autores (veja [Créditos](#créditos)).

## Sobre o projeto

A Lume Eventos é uma produtora boutique que vive de indicações e do Instagram, sem presença web própria. O site foi pensado para:

- passar credibilidade a quem chega por indicação;
- apresentar serviços e exibir um portfólio de eventos filtrável;
- gerar pedidos de orçamento qualificados (formulário + WhatsApp);
- permitir que a cliente atualize todo o conteúdo sozinha, pelo painel do WordPress.

O briefing completo está em [`docs/01-briefing.md`](docs/01-briefing.md).

## Funcionalidades

- Páginas: **Home, Sobre Nós, Serviços, Portfólio, Depoimentos e Contato**
- Portfólio com filtro por tipo de evento e página interna com galeria
- Conteúdo gerenciável via *Custom Post Types* (eventos, serviços e depoimentos)
- Formulário de contato com notificação por e-mail e botão flutuante de WhatsApp
- Layout responsivo (mobile first), acessível e otimizado para SEO e performance

## Tecnologias

| Área | Tecnologia |
|---|---|
| CMS | WordPress (tema em blocos / block theme) |
| Front-end | HTML, CSS, JavaScript |
| Blocos customizados | React (`@wordpress/scripts`) |
| Automação | Python (scripts auxiliares) |
| Design | Figma |
| Ambiente local | LocalWP + VS Code |
| Controle de versão | Git e GitHub |

## Estrutura do repositório

```
lume-eventos/
├── docs/        # briefing, wireframes e decisões de projeto
├── theme/       # tema WordPress (lume-theme)
├── scripts/     # utilitários em Python (ex.: otimização de imagens)
└── README.md
```

## Como rodar localmente

1. Instale o [LocalWP](https://localwp.com/) e crie um novo site WordPress.
2. Clone este repositório e copie (ou crie um link simbólico para) a pasta `theme/` em:
```
   wp-content/themes/lume-theme
```
3. No painel do WordPress, ative o tema **Lume**.
4. Instale os plugins necessários (formulário de contato, SEO, cache) conforme descrito em `docs/`.
5. Para desenvolver os blocos em React:
```bash
   cd theme
   npm install
   npm run start
```

## 🗺️ Roadmap

- [x] Briefing do projeto
- [ ] Wireframes e layout no Figma
- [ ] Configuração do ambiente (LocalWP + Git)
- [ ] Custom Post Types (portfólio, serviços, depoimentos)
- [ ] Desenvolvimento do tema e das páginas
- [ ] Formulário de contato e WhatsApp
- [ ] Responsividade, acessibilidade, SEO e performance (Lighthouse 90+)
- [ ] Publicação em hospedagem (domínio, SSL, cache e backup)
- [ ] Documentação de entrega e case no portfólio

## Demonstração

- Site publicado: _em breve_
- Protótipo no Figma: _em breve_

## Licença

Distribuído sob a licença **GPL-2.0-or-later**, em conformidade com o ecossistema WordPress. Veja o arquivo [`LICENSE`](LICENSE).

## Créditos

- Imagens: [Unsplash](https://unsplash.com/) e [Pexels](https://www.pexels.com/) (licença livre; autores listados em `docs/creditos.md`)
- Fontes: [Fraunces](https://fonts.google.com/specimen/Fraunces) e [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts

## Autor

**Gustavo Oki** — estudante de Engenharia de Software na UnB
[GitHub](https://github.com/GustOki) · [LinkedIn](www.linkedin.com/in/gustavooki)
