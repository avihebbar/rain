# rain

### Installing

```sh
# Download rain audio file
curl -O https://raw.githubusercontent.com/chunkhang/rain/master/rain.m4a

# Move file to ~/Music
mv rain.m4a ~/Music

# Append commands to ~/.zshrc
echo "\nfunction rain() {\n\techo Start raining...\n\tafplay -q 1 ~/Music/rain.m4a &\!\n}\n\nfunction sun() {\n\techo Stop raining...\n\tkillall afplay &>/dev/null\n}" >> ~/.zshrc

# Reload configuration
source ~/.zshrc
```

### Using

```sh
# Play rain in the background
rain

# Stop rain
sun
```
