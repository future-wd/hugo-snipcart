# Snipcart for HUGO

## Configuration

``` YAML
# config.yaml
Params:
  snipcart:
    enabled: true # defaults to true
    key: # your public API key. 
    side: true # or false for full screen cart
    bootstrap: true # enables snipcart z-index css for bootstrap compatibility 
```

## Installation

``` YAML
# config.yaml
module:
  imports:
  - path: github.com/future-wd/hugo-snipcart/v3
```

```HTML
<!-- baseof.html -->
<html>
  <head>
    {{ partialCached "snipcart/hints" . }}
    {{ partialCached "snipcart/css" . }}
    <title>...</title>
  </head>
  <body>
    ...
    {{ partialCached "snipcart/js" . }}
  </body>
</html>
```
