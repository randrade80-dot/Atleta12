# ATLETA 12 (PWA)
Arquivos: index.html, manifest.json, sw.js, icon.svg, icon-192.png, icon-512.png

## Executar no PC
cd atleta12 && python3 -m http.server 8080  -> abra http://localhost:8080
(Service worker e instalação exigem HTTPS ou localhost; abrir o arquivo com duplo clique funciona, mas sem instalação/offline.)

## Hospedar (HTTPS gratuito)
Envie a pasta para GitHub Pages, Netlify (arrastar e soltar) ou Cloudflare Pages.

## Android
1. Abra a URL HTTPS no Chrome. 2. Menu ⋮ > "Instalar app" / "Adicionar à tela inicial".
Os dados ficam no IndexedDB do aparelho/navegador. Limpar dados do site apaga tudo: exporte backups com frequência (Mais > Backup).

## Backup
Mais > Exportar backup (JSON, inclui fotos). Restaurar: Mais > Importar backup (pede confirmação e substitui os dados).

## Testes
Abra index.html#test: executa verificações de cálculo nutricional, validação numérica, backup e gráfico (resultado em aviso e console).

## Atualizar
O app usa cache offline: ao alterar arquivos, mude 'atleta12-v2' em sw.js.
