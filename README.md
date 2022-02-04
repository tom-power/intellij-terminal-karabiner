## Intellij Terminal Karabiner

Attempt to fix lack of support for native OSX shortcuts in intellij terminal, details [here](https://youtrack.jetbrains.com/issue/IDEA-153536)

### Installation

Install [karabiner-elements](https://karabiner-elements.pqrs.org/)

clone the project and import the rules

```
git clone git@github.com:tompower/intellij-terminal-karabiner.git \
&& cd ./intellij-terminal-karabiner \
&& ./install.sh
```

add the rules in karabiner

```
preferences -> complex modification -> add rule
find "intellij terminal native shortcuts" -> enable all
```

add some shortcuts in intellij

```
intellij -> preferences -> keymap

ctrl a -> Move caret to start line start
ctrl a + shift -> Move caret to line start with selection
ctrl e -> Move caret to line end
ctrl e + shift -> Move caret to end start with selection
ctrl c -> copy
ctrl k -> commit (and remove current)
```

### Notes

- option left/right, cmd l are working for me is so not included, please add if needed
- cmd u/l/k/c to ctrl u/l/k/c aren't covered in the ticket but are handy