# # 🎨 ArtGuide – Diretrizes Visuais do Projeto Nina Platformer

Este documento define **padrões visuais**, **tamanhos**, **escala**, **resoluções** e **regras de arte** do jogo Nina Platformer.  
O objetivo é garantir **consistência gráfica**, facilitar a criação de sprites e evitar retrabalho.

---

# 🧱 1. Estilo Visual do Jogo

**Estilo proposto:** Pixel Art  
**Resolução base:** Baixa resolução com pixels visíveis  
**Tema:** Aventura / Plataforma  
**Proporção:** 16:9

Motivos:  
- Combina com jogos 2D estilo plataforma  
- Fácil de produzir mesmo com equipe reduzida  
- Leve para exportação Web e mobile  
- Ótimo para animações simples  

---

# 📏 2. Escala e Resolução dos Sprites

## 📌 Tamanho dos Tiles
- **Tileset principal:** `32x32 px`
- **Colisões e grid:** 32px

Esse tamanho facilita level design e garante boa nitidez.

## 📌 Sprites do Player
- **Altura padrão:** `48 px`
- **Largura padrão:** `32 px`
- **Proporção humanoide estilizada**

### Animações sugeridas:
| Ação | Frames | Observações |
|------|--------|-------------|
| Idle | 4 | Movimentos sutis (cabelo, respiração) |
| Walk | 6–8 | Passo claro e suave |
| Jump | 1–2 | Um frame de pulo + caída opcional |
| Hurt | 2 | Piscada/contração |
| Death | 4 | Desvanecer ou queda |

---

# 🎨 3. Paleta de Cores

## 🎨 Paleta Base
Estilo recomendado: **cores vivas, contraste moderado e sombras suaves**.

### Tons principais:
- Azul vibrante  
- Rosa / magenta  
- Amarelo dourado  
- Verde esmeralda  
- Tons terrosos para cenários  

### Sites para gerar paletas consistentes:
- https://coolors.co  
- https://lospec.com/palette-list  
- https://palettegenerator.com  

### Iluminação:
- Evitar anti-alias manual (manter bordas pixeladas)  
- Sombras usando variação de tom e não blur  

---

# 🧩 4. Diretrizes de Cenário (Tilesets + Backgrounds)

## Tilesets (chão, paredes, plataformas)
- Tamanho: **32x32 px**
- Evitar excesso de detalhes (ruído visual)
- Utilizar 2–3 variações por terreno (para evitar repetição)
- Sombras simples (1 ou 2 tons mais escuro)

## Backgrounds
- Criar em **camadas** para parallax:
  - Camada 1 (fundo distante) — baixa saturação  
  - Camada 2 (montanhas / árvores) — tons médios  
  - Camada 3 (elementos próximos) — mais saturação  

### Resolução:
- Cada camada: múltiplos de `256px` ou `512px`  
- Modo Repeat habilitado para parallax  

---

# 🧍 5. Proporções dos Personagens

## Player  
- Altura: ~1,5 tiles (48 px)  
- Largura: ~1 tile (32 px)  

## Inimigos  
Tamanhos sugeridos:
- Pequenos: `32x32 px`  
- Médios: `48x48 px`  
- Grandes / chefes: `64x64 px` ou maior  

---

# ✏️ 6. Animação

### Regras gerais:
- FPS recomendado: **6 a 12 fps**  
- Animações curtas, loops suaves  
- Sem efeitos de blur (manter estética pixel art)  

### Dicas:
- Usar *squash & stretch* moderado  
- Priorizar silhueta clara  
- Menos detalhes = melhor leitura  

---

# 🎵 7. Efeitos Visuais (VFX)

## Partículas
- Gerar com sprites pequenos (8x8px ou 16x16px)
- Efeitos recomendados:
  - poeira no pulo  
  - brilho de coleta  
  - impacto ao tomar dano  
  - splash ao cair no chão  

## Transparências
- Usar transparência leve (20–40%), sem blur  
- Evitar gradientes complicados  

---

# 📁 8. Organização dos Arquivos de Arte

Use esta estrutura:

- assets/
- art/
- characters/
- player/
- enemies/
- tilesets/
- backgrounds/
- items/
- vfx/
- ui/


### Nomeação recomendada:
- `player_idle.png`  
- `slime_walk.png`  
- `tileset_terrain.png`  
- `bg_layer1.png`  
- `item_coin.png`  

Sempre: **snake_case**, sem espaços.

---

# 🧪 9. Teste de Arte na Godot

Sempre que adicionar um sprite:

1. Importar → Ajustar filtro para **Nearest**  
2. Desabilitar MipMaps  
3. Desabilitar Filter  
4. Verificar pivôs  
5. Testar tamanho no TileMap ou com o Player  

---

# ✔️ 10. Conclusão

Este guia serve para manter:
- Consistência visual  
- Facilidade de produção  
- Padronização entre sprites  
- Identidade clara do projeto  

Caso o estilo do jogo evolua, atualize este documento para manter tudo alinhado.


