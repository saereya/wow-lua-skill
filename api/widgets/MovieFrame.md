# MovieFrame

Widget methods (`SimpleMovieAPI`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplemovieapidocumentation.lua` (FileDataID 4637230)

## Methods

### EnableSubtitles

```lua
MovieFrame:EnableSubtitles(enable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### StartMovie

```lua
MovieFrame:StartMovie(movieID: number, looping: bool) -> success: bool, returnCode: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `movieID` | `number` |  |
| `looping` | `bool` | default `false` |

### StartMovieByName

```lua
MovieFrame:StartMovieByName(movieName: cstring, looping: bool, resolution: number) -> success: bool, returnCode: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `movieName` | `cstring` |  |
| `looping` | `bool` | default `false` |
| `resolution` | `number` | default `0` |

### StopMovie

```lua
MovieFrame:StopMovie()
```
