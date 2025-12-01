# 🗺️ Roadmap de Desenvolvimento – Nina Platformer Game
> **Objetivo:** Guiar a evolução do jogo de forma organizada, com etapas claras, prioridades e metas.

---

## 📌 1. Estrutura Inicial do Projeto
### Status: Em andamento
- [x] Criar repositório no GitHub  
- [x] Criar estrutura base de pastas  
- [ ] Definir convenções de nomes (snake_case)  
- [ ] Criar template inicial de cenas  
- [ ] Criar README com visão geral do projeto  

---

## 🎨 2. Arte e Diretrizes Visuais
### Objetivo: Definir identidade visual consistente antes de expandir o jogo.

- [ ] Definir paleta de cores do jogo  
- [ ] Definir estilo do player (pixel art? cartoon? 32x32?)  
- [ ] Criar documento `ArtGuide.md` com padrões:  
  - escala  
  - grid  
  - resolução dos sprites  
  - tamanho dos tiles (16px, 32px, 48px, etc.)  
- [ ] Criar sprites iniciais:  
  - [ ] Player (idle, walk, jump)  
  - [ ] Tileset básico de terreno  
  - [ ] Background simples para Level 1  

---

## 🧍 3. Personagem Principal (Player)
### Status: A iniciar

- [ ] Criar cena `Player.tscn`  
- [ ] Movimentação horizontal  
- [ ] Pulo  
- [ ] Checagem de chão com `RayCast2D`  
- [ ] Adicionar animações  
- [ ] Sistema de vida  
- [ ] Detecção de dano  

---

## 🏞️ 4. Cenários e Construção de Fases

- [ ] Criar `Level_01`  
- [ ] Criar sistema de Tilesets  
- [ ] Configurar colisões no tileset  
- [ ] Criar parallax background  
- [ ] Criar checkpoints  
- [ ] Criar `Level_02` com novas mecânicas  

---

## 🧠 5. Sistemas do Jogo (Core)

- [ ] Criar cena global `Game.tscn`  
- [ ] `GameManager` – carregar fases, reset, eventos  
- [ ] `InputManager`  
- [ ] `SaveSystem` (opcional – progresso, itens, vidas)  
- [ ] Sistema de áudio (sons + músicas)  

---

## 👾 6. Inimigos

- [ ] Criar inimigo base “Slime”  
  - [ ] Movimento patrol  
  - [ ] Dano ao player  
  - [ ] Morte  
- [ ] Criar inimigo avançado (voador, ataque à distância, etc.)  
- [ ] Criar `Enemy.gd` para herança  

---

## 💎 7. Itens & Mecânicas Extras

- [ ] Coletáveis (moedas, cristais, estrelas…)  
- [ ] Power-ups (pulo duplo, velocidade, vida extra)  
- [ ] Plataformas móveis  
- [ ] Portas / chaves  
- [ ] Armadilhas (espinhos, quedas)  

---

## 📺 8. Interface (UI)

- [ ] Criar HUD  
  - [ ] Vidas  
  - [ ] Itens coletados  
  - [ ] Timer (opcional)  
- [ ] Menu principal  
- [ ] Tela de pausa  
- [ ] Tela de game over  

---

## 📦 9. Polimento e Otimização

- [ ] Ajustar colisões (pixel-perfect)  
- [ ] Otimizar TileMap  
- [ ] Ajustar som e música  
- [ ] Melhorar feedback visual do player  
- [ ] Adicionar partículas (pulo, dano, morte)  

---

## 🚀 10. Build & Publicação

- [ ] Exportar para Windows  
- [ ] Exportar para Android  
- [ ] Exportar para Web (HTML5)  
- [ ] Testes  
- [ ] Beta externo  
- [ ] Publicação final  

---

## 📏 Progresso Geral

| Área | Status |
|------|--------|
| Estrutura do projeto | 🟡 Em andamento |
| Arte | ⚪ Não iniciado |
| Player | ⚪ Não iniciado |
| Inimigos | ⚪ Não iniciado |
| Cenários | ⚪ Não iniciado |
| UI | ⚪ Não iniciado |
| Sistemas principais | ⚪ Não iniciado |
| Publicação | ⚪ Não iniciado |

---

## 📜 Observações importantes

- Mantenha commits pequenos e frequentes  
- Use nomes de arquivos padronizados (snake_case)  
- Sempre mova arquivos pelo editor da Godot para evitar erros de referência  

