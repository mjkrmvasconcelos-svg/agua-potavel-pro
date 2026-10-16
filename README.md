# Água Potável Pro — versão atualizada

Aplicativo web responsivo para controle operacional de tratamento de água potável.

## Recursos
- Registro operacional de data/hora, operador, pH, turbidez e observações.
- Teste de proveta com cálculo de vazão em mL/min, L/min e L/h.
- Calculadora de consumo teórico para barrilha, sulfato de alumínio e cal hidratada.
- Cronômetros independentes para barrilha e sulfato de alumínio.
- Alerta sonoro ao completar 60 segundos em cada cronômetro (o navegador precisa permitir áudio; mantenha a página aberta para melhor funcionamento).
- Registro de volume em mL, vazão em mL/min e L/h e massa estimada usando densidade informada.
- Histórico local, exportação CSV e impressão/salvar como PDF.
- Cache offline básico via service worker.

## Como abrir
Abra `index.html` em navegador moderno. Para instalar como PWA, hospede em HTTPS (por exemplo, GitHub Pages) e use o menu do Chrome no Android para instalar/adicionar à tela inicial.

## Importante
Os dados ficam no armazenamento local do navegador e não sincronizam automaticamente entre aparelhos. Exporte o histórico regularmente. A densidade varia conforme produto e concentração; informe um valor confirmado na ficha técnica ou medição. O aplicativo não determina a dosagem ideal nem comprova potabilidade. Siga os procedimentos operacionais e as orientações do responsável técnico.

Este ZIP contém o código-fonte web, não um APK compilado.
