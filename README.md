# chrome-cookie-cutter

Very specific CLI utility for extracting specific cookie names from Chrome's cookie store, for re-use elsewhere in scripting.

## Install

```
go install github.com/saranrapjs/chrome-cookie-cutter
```


## Usage

Standalone:

```
chrome-cookie-cutter my-domain.com my-cookie-name
```

In conjunction with something like cURL + some kind of HTTP header auth:

```
curl -H "Authorization: Bearer `chrome-cookie-cutter my-domain.com my-cookie-name`" my-domain.com
```

### About

This is 100% derived from this [great script](https://gist.github.com/dacort/bd6a5116224c594b14db).
