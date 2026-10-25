# WeatherScript

Namespace `C_Weather` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/weatherscriptdocumentation.lua` (FileDataID 8346411)

Cloudy, with a chance of documentation.

## Functions

### GetCurrentWeather

```lua
C_Weather.GetCurrentWeather() -> info: WeatherInfo
```

C_Weather the outlook is favorable.

## Events

### WEATHER_CHANGED

```lua
WEATHER_CHANGED()
```

The weather has taken a turn.

`UniqueEvent`

## Types

### WeatherInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `WeatherType` | default `"Clear"` |
| `intensity` | `number` |  |
