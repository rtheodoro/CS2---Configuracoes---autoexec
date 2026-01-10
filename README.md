# CS2 - Configurações de Jogo e Treino 
Minhas configurações para jogar Counter-Strike 2. [Como Usar](#como-usar)

To enable this config in practice mode: `exec autoexec; mp_restartgame 1` 

Crosshair code: `CSGO-bMBxd-4XfA6-xPOLq-SVEBJ-knhrM`

## Key Bindings

### Movement
| Action | Key | 
|--------|-----|
| Duck | `shift` | 
| Jump | `space` | 
| Jump | `mwheeldown` | 
| Walk | `capslock` | 
| Radar Zoom | `crtl` | 

### Grenades
| Grenade Type | Key | 
|--------------|-----|
| Flashbang | `x` |
| Smoke Grenade | `c` |
| Molotov | `v` |

### Utility
| Action | Key | Note |
|--------|-----|------|
| Drop C4 | `Mouse5` | Automatically announces in team chat |

## Features

### HUD Settings
- **Screen brightness**: 2.4
- **HUD scaling**: 1.0
- **Target ID**: Enabled (shows enemy identification on screen)
- **Equipment display**: Always visible
- **Build info**: Hidden

### Radar
- **Radar scale**: 0.3
- **Teammate colors**: Enabled

### Viewmodel
- **Preset position**: 3 (Classic viewmodel)

### Other Settings
- **Silencer mode**: Prevents accidental silencer removal
- **X-ray in spectator**: Enabled
- **Random weapons in DM**: Disabled
- **Teammate overhead info**: Mode 3 with colors

## Training Configuration

This configuration includes settings optimized for practice mode:

- Cheats enabled
- No auto-kick
- No team balance
- Extended round time (10000 seconds)
- Zero freeze time
- Buy anywhere on map
- Maximum starting money ($65535)
- Unlimited grenades and utility
- Infinite ammo
- Grenade trajectory visible for 10 seconds
- Healthshot heals 100 HP

## Notes

- All training commands require `sv_cheats 1` to be active

#### Como usar

Passo a Passo
1. Localize a Pasta cfg 
O local exato no Linux pode variar, mas geralmente segue um caminho semelhante a este dentro do seu diretório Steam:
~/.steam/steam/steamapps/common/Counter-Strike Global Offensive/game/csgo/cfg/ 
Você pode encontrar facilmente a pasta correta através do Steam: 

    Abra o Steam e vá para a sua Biblioteca.
    Clique com o botão direito em Counter-Strike 2 e selecione `Propriedades > Arquivos Instalados > Explorar`.
    Na janela do explorador de arquivos que abrir, navegue até a pasta `game > csgo > cfg`. 

2. Crie o Arquivo autoexec.cfg 

    Na pasta cfg, clique com o botão direito e crie um novo Documento de Texto.
    Renomeie o arquivo para `autoexec.cfg`. Certifique-se de que a extensão .txt não permaneça oculta (ative a visualização de extensões de arquivo se necessário).
    Abra o arquivo `autoexec.cfg` com um editor de texto simples. 

3. Adicione Comandos
Digite ou cole os comandos de console que você deseja executar automaticamente, cada um em uma nova linha. Por exemplo, você pode adicionar comandos para a sua mira, binds de pulo, configurações de áudio, etc. 
Dica Importante: Adicione host_writeconfig no final do seu arquivo autoexec.cfg. Isso garante que o jogo salve quaisquer alterações feitas pelos comandos do seu autoexec nas suas configurações padrão permanentes. 
4. Configure as Opções de Lançamento do Steam
Para garantir que o autoexec.cfg seja executado automaticamente toda vez que você iniciar o CS2, você precisa adicionar um comando nas opções de lançamento do jogo no Steam: 

    Na Biblioteca do Steam, clique com o botão direito em Counter-Strike 2 e selecione Propriedades.
    Na aba Geral, na seção Opções de Lançamento, digite o seguinte comando:
    `+exec autoexec.cfg` 

