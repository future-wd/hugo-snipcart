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
<!-- baseof.html  the js is deferred so it can be called in the head for faster load -->
<html>
  <head>
    {{ partialCached "snipcart/hints" . }}
    {{ partialCached "snipcart/css" . }}
    {{ partialCached "snipcart/js" . }}
    <title>...</title>
  </head>
  <body>
    ...
  </body>
</html>
```
