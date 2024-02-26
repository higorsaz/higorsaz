### Olá, eu sou o Higor! 🤙


![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra&theme=dark&show_icons=true)
\`\`\`


      if (line.includes(REPO_CARD_TABLE_FLAG)) {
        return generateTable({ isRepoCard: true });
      }
      if (line.includes(STAT_CARD_TABLE_FLAG)) {
        return generateTable({ isRepoCard: false });
      }
      return line;
    })
    .join("\n");
};

fs.writeFileSync(TARGET_FILE, buildReadme());
