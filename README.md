# samilbulur-website

`samilbulur.com` kişisel sitesi. [Astro](https://astro.build) ile statik üretilir, sıfır JavaScript gönderir.

## Komutlar

| Komut | Ne yapar |
|---|---|
| `npm install` | Bağımlılıkları kurar (Node ≥ 22.12) |
| `npm run dev` | Yerel sunucu, `localhost:4321` |
| `npm run build` | `dist/` altına statik site üretir |
| `npm run preview` | Build çıktısını yerelde sunar |

## Yapı

- `src/pages/index.astro` — ana sayfa
- `src/content/blog/*.md` — blog yazıları; frontmatter şeması `src/content.config.ts` içinde
- `src/layouts/Base.astro` — ortak iskelet ve stil

Yeni yazı: `src/content/blog/` altına `.md` dosyası ekle (örnek: `ornek-yazi.md`). `draft: true` olanlar yayınlanmaz ama repo halka açık olduğu için GitHub'da görünür.

## Yayın

Henüz yayında değil. Plan: Cloudflare Pages, build `npm run build`, çıktı `dist` — ayrıntılar `~/samilProjects/infra/handbook/01-alan-adi-el-kitabi.md` §6.4.
