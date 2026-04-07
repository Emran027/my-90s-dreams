# 90's Dream - Game Specification

## 1. Project Overview
- **Name**: 90's Dream
- **Tagline**: By Emran Hossain
- **Type**: 2D Side-scrolling Platformer (Web)
- **Core Style**: Retro 90s aesthetic with neon, checkerboard, pixel art

## 2. Visual Specification

### Color Palette
- **Background**: Deep purple to black gradient (#1a0a2e → #0d0015)
- **Neon Pink**: #FF00FF (accents, UI)
- **Neon Cyan**: #00FFFF (player, highlights)
- **Neon Green**: #39FF14 (coins, positive elements)
- **Neon Yellow**: #FFFF00 (stars, special)
- **Grid/Checkerboard**: Magenta/purple checkerboard pattern

### Visual Effects
- CRT scanline overlay effect
- Screen flicker on impacts
- Chromatic aberration on game over
- Pixel-perfect rendering
- Neon glow on all UI elements
- Starfield with different layers
- Platform pixel art with brick patterns

### Player Character
- 32x32 pixel sprite
- Cyan with magenta outline
- Trail effect with afterimages
- Jump dust particles

## 3. Gameplay Features

### Controls
- Arrow keys / WASD for movement
- Space/Up/W to jump
- Mouse/touch: left third = left, right third = right, middle = jump

### Mechanics
- **Coins**: Collect for points (+10 each)
- **Power-ups**:
  - ⭐ Star: Invincibility for 5 seconds
  - ⚡ Lightning: Speed boost for 5 seconds
  - ❤️ Heart: Extra life
- **Enemies**:
  - Red slime blobs (patrol platforms)
  - Spike balls (fall from top)
- **Hazards**: Bottomless pit = death

### Scoring System
- Distance: 1 point per 10px
- Coins: 10 points each
- Enemy jump-kill: 50 points
- Combo multiplier: consecutive coins within 2s = 2x, 3x, 4x
- High score saved to localStorage

### Game States
1. **Title Screen**: Logo, "Press SPACE to Start", high score
2. **Playing**: Active gameplay
3. **Paused**: Press P to pause
4. **Game Over**: Score display, restart option

## 4. Audio (Visual Representation)
- Visual "sound waves" on coin collect
- Screen shake on damage
- Flash effects for power-ups

## 5. UI Elements
- Score (top-left) with retro LCD font style
- High Score (top-right)
- Power-up indicator (below score)
- Lives display (heart icons)
- Distance meter

## 6. Technical Improvements
- Smooth 60fps with requestAnimationFrame
- Object pooling for particles/platforms
- Efficient collision detection
- Mobile responsive with touch zones

## 7. Acceptance Criteria
- [ ] Full screen immersive experience
- [ ] 90s neon aesthetic clearly visible
- [ ] Multiple power-ups functional
- [ ] Enemies with patrol AI
- [ ] Combo scoring system
- [ ] Lives system with respawn
- [ ] "90's Dream By Emran Hossain" branding
- [ ] Touch and keyboard controls
- [ ] High score persistence
- [ ] CRT/retro visual effects