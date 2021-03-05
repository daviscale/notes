# Shell Notes

## Handy Shell One-Liners

### Project Wide Find/Replace

```
ag --js 'thingToFind' | grep -o 'src\/path.*js' | xargs sed -i '' 's/thingToFind/replaceWith/g'
```
TODO: Make it so that `thingToFind` only has to be used once.
