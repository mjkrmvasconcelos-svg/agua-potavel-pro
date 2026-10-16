# Água Potável Pro — versão inicial

Aplicativo web instalável (PWA) para controle operacional de tratamento de água potável.

## Recursos
- Registro operacional com data/hora, operador, pH, turbidez e observações.
- Teste de proveta: volume coletado e tempo para calcular vazão em L/min e L/h.
- Cálculo de consumo teórico de barrilha, sulfato de alumínio e cal hidratada (Tina), usando dosagem aprovada em mg/L, vazão de água e horas de operação.
- Cronômetros independentes para barrilha e sulfato, com iniciar, pausar, zerar e salvar o tempo no histórico.\n- Histórico salvo localmente no dispositivo.
- Exportação CSV e impressão/salvar como PDF pelo navegador.
- Interface responsiva e cache offline básico.

## Como abrir
Abra `index.html` em um navegador moderno. Para instalação PWA com funcionamento offline completo, hospede em HTTPS (por exemplo, GitHub Pages) e abra a página pelo Chrome no Android; use o menu do navegador e escolha **Instalar app** ou **Adicionar à tela inicial**.

## Sobre o APK
Este ZIP contém o código-fonte da aplicação web, não um APK compilado. A compilação de APK requer ambiente Android/Android Studio e assinatura. O APK não foi compilado neste ambiente porque não há Android SDK/Gradle instalado. O projeto pode ser empacotado como APK em uma etapa posterior.

## Fórmulas
- Vazão medida: `L/min = volume_mL / tempo_segundos * 60 / 1000`
- Consumo teórico: `kg/dia = dose_mg_L * vazão_m3_h * horas_dia / 1000`
- Consumo por hora: `kg/h = dose_mg_L * vazão_m3_h / 1000`

A fórmula de consumo pressupõe que a dosagem informada esteja expressa em mg/L como produto equivalente. Para soluções preparadas, é necessário considerar concentração real, densidade e pureza. O resultado não substitui ensaio de tratabilidade, procedimento operacional aprovado ou orientação de profissional habilitado. O app não determina automaticamente dosagem ideal nem comprova potabilidade.

## Privacidade e limitações
Os dados ficam no armazenamento local do navegador neste dispositivo. Limpar os dados do navegador pode apagar o histórico. Exporte relatórios regularmente. Esta é uma versão inicial; autenticação, sincronização entre aparelhos e backup automático ainda não estão incluídos.
