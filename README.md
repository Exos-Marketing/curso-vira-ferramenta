# Curso vira ferramenta

Skill do Claude que transforma o seu curso em **ferramentas web próprias**: calculadoras, geradores, checklists, diagnósticos e planners que o aluno usa para aplicar o seu método, e que você pode vender ou usar para captar alunos.

Você entrega o nome do curso e a transcrição das aulas. O Claude:

1. lista o que o curso ensina e o que é repetitivo ou manual para o aluno;
2. pesquisa o mercado: quem é o aluno, o que ele já paga, que apps existem e onde falham;
3. sugere de 5 a 10 ferramentas, com monetização e preço para o Brasil;
4. ranqueia e escolhe a nº 1;
5. constrói a nº 1 com você: telas, código pronto, como testar e onde publicar de graça;
6. entrega as próximas ferramentas e um plano de 30 dias para lançar.

> "Tudo o que puder ser software, será software." João Pedro Resende, CEO da Hotmart, no FIRE 2026.

## Jeito mais rápido: só o prompt

Não quer instalar nada? Abra o [prompt.md](prompt.md), copie, troque o nome do curso e cole a transcrição em qualquer chat do Claude.

## Instalar a skill

**Claude Code**

```bash
git clone https://github.com/Exos-Marketing/curso-vira-ferramenta.git
mkdir -p ~/.claude/skills
cp -r curso-vira-ferramenta/curso-vira-ferramenta ~/.claude/skills/
```

Depois é só pedir: *"transforma meu curso em ferramenta, a transcrição está na pasta aulas/"*.

**Claude.ai (site ou app)**

1. Baixe este repositório: botão verde **Code → Download ZIP**.
2. Compacte só a pasta `curso-vira-ferramenta` (a de dentro, com o `SKILL.md`) num `.zip`.
3. Em **Configurações → Capacidades → Skills**, clique em **Enviar skill** e escolha o `.zip`.

## Do que você precisa

- **A transcrição das aulas.** Se só tiver os vídeos, transcreva antes (a transcrição automática do YouTube ou do Google Drive resolve).
- **Uma conta do Claude.** A pesquisa de mercado fica melhor com a busca na web ligada.
- **Publicar a ferramenta é de graça** (GitHub Pages, Vercel ou Replit). Cobrar depende da sua plataforma (Hotmart, Kiwify, Stripe), com as taxas dela.

## Limites

- A skill organiza e aplica o que o seu curso ensina. Em saúde, direito e finanças, a ferramenta não dá diagnóstico, dose ou parecer, e avisa isso na tela.
- Preço e mercado são estimativas a partir de pesquisa; valide com seus alunos antes de lançar.

---

Mantido pela [Exos Marketing](https://github.com/Exos-Marketing). Licença MIT.
