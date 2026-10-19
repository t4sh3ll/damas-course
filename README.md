# Damas Pro - Curso Interativo

## 🎓 Sobre o Projeto

Curso interativo baseado no banco de dados extraído do **Damas Pro v11.16.0** (APK profissional de Damas Brasileiras).

## 🌐 Online no GitHub Pages

✅ **Site ativo**: https://t4sh3ll.github.io/damas-course/

- 100% frontend (HTML/CSS/JS)
- Sem backend necessário
- Funciona em qualquer navegador
- Progresso salvo no localStorage

---

## 📊 Banco de Dados Extraído

### Origem
- **APK**: Damas.ver.11.16.0.build.108.apk
- **Package**: mkisly.checkers.damas.brazilian
- **Técnica**: REA + JADX (descompilação)

### Estrutura
```
assets/mtw/
├── db11b.dat (992B)     - 248 posições - Aberturas rápidas
├── db12b.dat (14.8KB)   - 3,720 posições - Combos fáceis
├── db13b.dat (143.8KB)  - 35,960 posições - Combos médios
├── db21b.dat (14.8KB)   - 3,720 posições - Jogos pretas
├── db21w.dat (14.8KB)   - 3,720 posições - Jogos brancas
├── db22b.dat (215.7KB)  - 53,940 posições - Banco principal ⭐
└── db31b.dat (143.8KB)  - 35,960 posições - Versão texto
```

**Total**: 137,268 posições extraídas

### Formato dos Dados
Cada valor é um **bitmask** representando peças no tabuleiro:
- `Valor 1` = peça na casa A8 (bit 0)
- `Valor 2` = peça na casa B8 (bit 1)
- `Valor 4` = peça na casa C8 (bit 2)
- `Valor 771` = peças em A8, B8, A7, B7 (bits 0,1,8,9)

---

## 🎮 Funcionalidades do Curso

### 1. Tabuleiro Interativo
- Renderização 8x8 com peças visuais
- Destaque de movimentos válidos
- Animações suaves
- Design responsivo

### 2. Sistema de Combinações
| Nível | Quantidade | Descrição |
|-------|------------|-----------|
| 🟢 Fácil | 3 | Capturas básicas, promoções |
| 🟡 Médio | 4 | Sacrifícios, controle central |
| 🔴 Difícil | 3 | Zig-zag, pinças, finais |

### 3. Progresso e Conquistas
- Salvo automaticamente no localStorage
- Barra de progresso visual
- Indicador de combinações completas
- Sistema de conquistas (em desenvolvimento)

### 4. Ferramentas de Aprendizado
- **Dica**: Mostra explicação da combinação
- **Resolver**: Demonstra a solução completa
- **Anterior/Próximo**: Navegação entre combinações
- **Histórico**: Lista de movimentos realizados

---

## 🚀 Como Usar

### Para Estudantes
1. Acesse https://t4sh3ll.github.io/damas-course/
2. Selecione uma combinação na lista lateral
3. Clique na peça branca para selecionar
4. Clique no destino para mover
5. Complete a sequência para vencer
6. Use "Dica" se precisar de ajuda

### Para Desenvolvedores
```bash
# Clone o repositório
git clone https://github.com/t4sh3ll/damas-course.git

# Abra index.html no navegador
# Ou hospede em qualquer servidor estático
```

---

## 📂 Estrutura do Projeto

```
damas-course/
├── index.html          # Aplicação completa (30KB)
├── README.md           # Esta documentação
└── .github/
    └── workflows/      # CI/CD (future)
```

**Tecnologias**: HTML5, CSS3, JavaScript vanilla
**Dependências**: Nenhuma (100% standalone)

---

## 🎯 Combinações Incluídas

### Fácil
1. **Captura Dupla Clássica** - Movimento básico de captura
2. **Dominação Central** - Controle do centro
3. **Ataque em X** - Ameaças múltiplas

### Médio
4. **Sacrifício Estratégico** - Ofereça peça para ganhar posição
5. **Promoção com Captura** - Promova enquanto captura
6. **Pinça Lateral** - Restrinja movimentos inimigos
7. **Conversão de Final** - Vire vantagem em vitória

### Difícil
8. **Zig-Zag Tático** - Capturas alternadas
9. **Fuga em Cascata** - Escape de armadilhas
10. **Bloqueio Total** - Imobilize o adversário

---

## 💡 Diferenciais

### vs App Original
- ✅ **Interativo**: Jogável, não apenas visualização
- ✅ **Educacional**: Dicas e explicações
- ✅ **Progresso**: Acompanhamento de aprendizado
- ✅ **Gratuito**: Sem anúncios ou compras

### vs Outros Cursos
- ✅ **Baseado em dados reais**: Extraído do APK profissional
- ✅ **137K+ posições**: Maior banco disponível
- ✅ **Offline**: Funciona sem internet após carregado
- ✅ **Responsivo**: Funciona em mobile e desktop

---

## 🔧 Instalação Local

### Opção 1: Servidor Estático Simples
```bash
python3 -m http.server 8000
# Acesse http://localhost:8000
```

### Opção 2: GitHub Pages (Recomendado)
1. Faça fork do repositório
2. Ative GitHub Pages em Settings
3. Pronto! Site estará em https://seuuser.github.io/damas-course/

### Opção 3: Netlify/Vercel
```bash
# Deploy automático ao push
netlify deploy --prod
```

---

## 📊 Estatísticas

| Métrica | Valor |
|---------|-------|
| Posições extraídas | 137,268 |
| Combinações disponíveis | 10 |
| Tamanho do app | 30 KB |
| Dependências | 0 |
| Tempo de carregamento | <1s |
| Suporte mobile | ✅ |

---

## 🛠️ Tecnologias

- **Frontend**: HTML5, CSS3, JavaScript ES6+
- **Build**: Nenhuma (single file)
- **Deploy**: GitHub Pages
- **Storage**: localStorage (progresso)

---

## 📝 License

MIT License - Use livremente para estudos e projetos educacionais.

---

## 🤝 Contribuições

1. Fork o repositório
2. Crie branch (`git checkout -b feature/nova-combinacao`)
3. Commit mudanças (`git commit -am 'Adiciona nova combinação'`)
4. Push (`git push origin feature/nova-combinacao`)
5. Abra Pull Request

---

**Criado por**: ML Soluções Tecnológica  
**Data**: Outubro 2026  
**Versão**: 1.0.0

---

*Curso baseado em análise REA do APK Damas Pro v11.16.0*
