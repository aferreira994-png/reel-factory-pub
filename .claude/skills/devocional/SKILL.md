---
name: devocional
description: Gera o devocional diário de oração do usuário. Use quando o usuário invocar /devocional ou pedir seu devocional, oração diária ou meditação bíblica. O argumento (se houver) é o tema ou a oração do dia.
---

# Devocional Diário

Você vai preparar o devocional diário do usuário, em português, com tom acolhedor, pastoral e pessoal — como um momento de oração, não como um artigo.

## Como gerar

1. **Tema**: use o texto passado como argumento (ex.: `/devocional senhor eu preciso ouvir a sua voz`). Se nenhum tema for passado, escolha um tema edificante ligado ao dia a dia (confiança, gratidão, descanso, direção, perseverança).
2. **Estrutura do devocional**:
   - **Título** curto ligado ao tema.
   - **Versículo-chave**: um versículo bíblico central, citado com a referência (ex.: 1 Samuel 3:10). Escolha um versículo realmente pertinente ao tema.
   - **Reflexão**: 3 a 5 parágrafos curtos meditando sobre o versículo e o tema, aplicados à vida real. Fale diretamente com o leitor ("você"). Evite clichês e jargão religioso vazio.
   - **Para meditar hoje**: 2 ou 3 perguntas ou passos práticos para o dia.
   - **Oração**: uma oração em primeira pessoa (4 a 8 linhas), retomando o tema e o pedido do usuário com as palavras dele quando fizer sentido.
3. **Registro**: salve o devocional em `devocionais/AAAA-MM-DD-slug-do-tema.md` na raiz do repositório (crie a pasta se não existir), usando a data de hoje. Adicione também uma linha na tabela do índice `devocionais/README.md` (data, tema, versículo-chave, link do arquivo), criando a seção do mês se necessário. Depois, faça commit e push na branch de trabalho da sessão.
4. **Página web (Artifact)**: atualize a página "Meus Devocionais Diários" publicada em `https://claude.ai/code/artifact/bdfac1be-8cf0-4de9-a2f4-cadcda2412ea` — use a ferramenta Artifact passando essa URL no parâmetro `url` para manter o mesmo link. Adicione o devocional novo no topo (o mais recente aparece primeiro, completo) e acrescente a linha correspondente na tabela "Índice por dia". Mantenha o favicon 📖 e o design existente da página.
5. **Resposta ao usuário**: apresente o devocional completo na conversa (não apenas o caminho do arquivo) e lembre o link da página.

## Tom

- Caloroso, esperançoso e bíblico, sem ser sentimentalista.
- Se o tema trazido pelo usuário expressar dor, cansaço ou angústia, acolha isso na reflexão e na oração antes de apontar esperança.
