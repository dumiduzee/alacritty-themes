
# Alacritty Theme For Arch
Intelligence alacritty configuration and theming


## Installing Alacritty and Fish
### Installing Alacritty
```bash
  sudo pacman -S --needed alacritty
```
#### Installing Alacritty
```bash
  mkdir -p ~/.config/alacritty/themes
  git clone https://github.com/alacritty/alacritty-theme ~/.config/alacritty/themes
```
#### Install a Nerd Font.
```bash
  sudo pacman -S --needed ttf-jetbrains-mono-nerd
  yay -S ttf-hack-nerd 
```

### Add a default config for alacritty.

```bash
  cd $home
  git clone https://github.com/dumiduzee/alacritty-themes.git
```

### Add a default config for alacritty.

```bash
  cp -r alacritty-theme/alacritty/alacritty.toml ~/.config/alacritty/alacritty.toml
```

## Installing Fish


```bash
  sudo pacman -S --needed fish
```
### Add a default config file for fish.

```bash
  mkdir -p ~/.config/fish/config.fish
  cp alacritty-theme/fish/config.fish ~/.config/fish/config.fish
```

### Install eza, a replacement for ls.
```bash
  sudo pacman -S --needed eza
```

### Install starship shell prompt.
```bash
  sudo pacman -S --needed starship
```

### Build and install shell-color-scripts.
```bash
  git clone https://gitlab.com/dwt1/shell-color-scripts.git ~/alacritty-theme/
  cd shell-color-scripts
  makepkg -i
```

### Change the user default shell.
```bash
  chsh -s /bin/fish
```

## Config colourscript.

### Show all available colourscripts

```bash
  colorscript -a
```

### Run random colour script

```bash
  colorscript -r
```

### change colourscript from ```config.fish```

```bash
  nano ~/.config/fish/config.fish
```

### change this line ```config.fish```

```bash
  colorscript -e {YOUR_DESIRED_THEME}
```
#### Example

```colorscript -e zwaves```