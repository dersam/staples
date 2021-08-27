# Staples Theme

![Screenshot](/sample.png?raw=true)

Based on oh-my-zsh's `bureau` theme.  I liked bureau's two-line layout; while having the current working directory visible is great, I always disliked that long paths would cramp the space to actually write commands.

On smaller terminals, it looks like there's not that much space with the right hand side, but it will automatically disappear if you start to run into it while typing.

Like `bureau`, the git status is displayed on the right hand side, although the colors and icons were tweaked slightly.

It's called Staples because `Bureau en Gros` is the name of Staples (the office supply store) in Québec, and I like lame wordplay.

## Customizations
### Context Tags
Adds context sensitive tags to the righthand prompt, if conditions are met. This is currently all based on whether files exist in the current directory, but there's no reason it needs to be limited to that. `get_usables` can be modified
to add additional tags. See below list for files checked and the tags they generate.

- `<gulp>`: `gulpfile.js`
- `<composer>`: `composer.json`
- `<npm>`: `package.json`
- `<vagrant>`: `VagrantFile`
- `<bundler>`: `Gemfile`

### SSH status
If connected through an ssh session, displays `username@hostname` on the left second line before the prompt.

### Last command status
If the last exit code is non-zero, the `Z` in the prompt will turn red.
