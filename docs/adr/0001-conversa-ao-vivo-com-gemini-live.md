# Conversa ao vivo com Gemini Live, não com o Claude

A Conversa precisa ser fluida, com resposta em cerca de 1 segundo, e a conversa por turnos (gravar, enviar, gerar texto, gerar áudio) levava de 3 a 6 segundos por fala. Por isso a Conversa passa a usar o Gemini Live (voz em tempo real), aceitando custo por minuto (cerca de R$ 0,60 a R$ 1,80 por conversa de 10 minutos, com teto de R$ 50 por mês para os dois usuários) e trocando o "cérebro" da conversa do Claude para o Gemini. O Claude continua gerando as Aulas faladas, as Cenas e o resumo de correções do fim da Conversa. O navegador fala direto com o Gemini usando uma chave temporária gerada pelo Apps Script, para não exigir um servidor novo.

## Considered Options

- Conversa por turnos com o Claude: custo quase zero, mas a espera quebra o ritmo da conversa.
- Servidor próprio intermediando o áudio: mais controle, mas mais uma peça para manter.
