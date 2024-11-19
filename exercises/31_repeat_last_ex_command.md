### Repeat last ex command

`:bn` - move to the next buffer
`@:` - repeat the last ex command
`@@` - repeat the previous `@{0-9a-z":*}`

If you press `@@` before `@:` you will get an error because there is no `@{0-9a-z":*}` command to repeat.
