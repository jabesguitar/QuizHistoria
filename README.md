# Quiz História — Viagem no Tempo (6º ano)

Aplicativo Android educativo baseado nas 32 fotografias do material SAE Digital enviadas para este projeto. O app foi estruturado para uso offline, sem anúncios e sem cadastro.

## Conteúdo didático
- Idade Média: séculos V a XV; Alta Idade Média (V–X) e Baixa Idade Média (XI–XV).
- Reinos germânicos e Reino Franco: Clóvis, Pepino, o Breve, Carlos Magno e Tratado de Verdun.
- Igreja, mosteiros, clero regular e secular, monges copistas, manuscritos e iluminuras.
- Feudalismo, estamentos, feudo, suserania e vassalagem, obrigações servis.
- Revolução agrícola, burgos, guildas, corporações de ofício e feiras.
- Cruzadas, Inquisição e crise do século XIV.

## Recursos
- Resumo dividido em cinco áreas.
- Quiz principal com banco de 36 perguntas embaralhadas a cada partida.
- Fácil: 90 segundos por pergunta e 3 vidas.
- Normal: 60 segundos por pergunta e 4 vidas.
- Difícil: 30 segundos por pergunta e 5 vidas.
- Dica, efeitos sonoros simples, pular pergunta (ela vai para o fim da fila) e retorno ao início.
- Jogos alternativos: memória, verdadeiro ou falso, associação, caça-palavras e palavras cruzadas.
- Ícone Android próprio e identidade visual manteiga/cacau/azul elétrico.

## Gerar APK pelo GitHub
1. Crie um repositório novo no GitHub chamado `QuizHistoria` (ou outro nome).
2. Envie **todo o conteúdo desta pasta** para a raiz do repositório, incluindo `.github`.
3. Abra a aba **Actions** e permita a execução dos workflows, se o GitHub solicitar.
4. Execute **Build Quiz Historia APK** em `Run workflow` ou faça um push na branch `main`.
5. Quando terminar com sucesso, abra a execução e baixe o artefato **Quiz-Historia-APK**.
6. Extraia o ZIP baixado e instale `app-debug.apk` no Android. Se necessário, autorize a instalação de aplicativos dessa origem.

## Compilar localmente
Requer JDK 17 e Gradle 8.9:

```bash
gradle assembleDebug
```

O APK será gerado em `app/build/outputs/apk/debug/app-debug.apk`.

## Observações importantes
- O APK de depuração é apropriado para testes e instalação direta. Para distribuição pública, gere uma versão release assinada com uma chave própria.
- O app é uma primeira versão funcional do jogo. Os mini jogos de caça-palavras e palavras cruzadas são atividades simplificadas; o caça-palavras marca a lista de termos e as palavras cruzadas são preenchidas por resposta textual, não por uma grade cruzada tradicional.
- O conteúdo acompanha as páginas fotografadas; temas não visíveis no material enviado não foram acrescentados como conteúdo principal.


## Atualização 1.1.0
- Corrigida a abertura e a correspondência das cartas do jogo da memória.
- Reformulado o Verdadeiro ou Falso: cada rodada apresenta uma pergunta histórica e uma resposta proposta para o aluno julgar.
- Adicionadas trilhas instrumentais originais sintetizadas localmente para as telas, abas e minijogos, com reprodução/pausa, volume e mudo.
- Mantidos efeitos sonoros de acerto e erro com controle independente.
- Trilhas variam a sequência a cada entrada na tela e funcionam offline, sem arquivos externos de áudio.


## Versão 1.2.0 — Ilustrações no resumo

Foram adicionadas seis ilustrações originais, armazenadas localmente em `app/src/main/assets/images/`, nos tópicos de linha do tempo, Alta Idade Média, feudalismo e Baixa Idade Média. As ilustrações são recursos visuais didáticos, não fotografias documentais nem reproduções de imagens do livro.
