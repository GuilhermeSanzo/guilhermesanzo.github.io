# 🌐 guilhermesanzo.me — Portfólio & Página de Transição

Repositório da página institucional e temporária de transição do desenvolvedor **Guilherme Souza**, hospedada via **GitHub Pages** e vinculada ao domínio customizado [guilhermesanzo.me](https://guilhermesanzo.me).

---

## 📌 Contexto da Migração
Devido ao término do plano promocional de créditos na DigitalOcean, a infraestrutura original foi colocada em processo de migração. Durante este período, esta página estática moderna e responsiva atua como o ponto central de contato, links profissionais e vitrine dos projetos em destaque.

---

## 🎨 Design e Identidade Visual
* **Paleta & Tema**: Dark mode minimalista inspirado na paleta `zinc-950` com acentos em `zinc-800` e tipografia Inter/Geist Sans.
* **Identidade de Marca**: Logotipo oficial pessoal (`img/guilherme-logo.png`) e favicons vetoriais.
* **Aviso de Status**: Badge animada indicando status de migração e reconstrução de infraestrutura.
* **Cards de Projetos**: Vitrine com logos oficiais integrados:
  * **Frozen Fitness** (`img/frozen-logo.png`): E-commerce Laravel 11 com Tailwind CSS v4.
  * **Livraria Woody Woodpecker** (`img/woody-logo.png`): E-commerce moderno com Eloquent ORM.
* **Rodapé**: Ícones em SVG inline com links diretos para GitHub, LinkedIn, Currículo em PDF e e-mail de contato.
* **Responsividade**: Layout adaptável para desktop e mobile, com quebra otimizada para o cabeçalho acadêmico da FATEC-SP.

---

## 🌐 Configuração de DNS & Hospedagem (Namecheap + GitHub Pages)

### 1. Registros de DNS no Namecheap
| Tipo | Host | Valor / Destino | TTL |
|---|---|---|---|
| `A Record` | `@` | `185.199.108.153` | Automático |
| `A Record` | `@` | `185.199.109.153` | Automático |
| `A Record` | `@` | `185.199.110.153` | Automático |
| `A Record` | `@` | `185.199.111.153` | Automático |
| `CNAME Record` | `www` | `guilhermesanzo.github.io.` | Automático |

### 2. Configuração no GitHub Pages
* **Source**: Branch `main`, diretório raiz (`/`).
* **Custom Domain**: `guilhermesanzo.me` (persistido pelo arquivo [`CNAME`](CNAME)).
* **Segurança**: Certificado SSL/TLS via Let's Encrypt com `Enforce HTTPS` ativado.

---

## 📂 Estrutura de Arquivos
```text
guilhermesanzo.github.io/
├── img/
│   ├── frozen-logo.png      # Logo do projeto Frozen Fitness
│   ├── guilherme-logo.png     # Logo pessoal Guilherme Souza
│   └── woody-logo.png       # Logo do projeto Woody Woodpecker
├── CNAME                    # Apontamento de domínio customizado (guilhermesanzo.me)
├── favicon.svg              # Ícone do site para navegadores
├── index.html               # Página única com Tailwind CSS inline e scripts
└── README.md                # Documentação técnica de arquitetura e DNS
```
