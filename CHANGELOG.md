# Changelog

<!--next-version-placeholder-->

## v1.1.0 (2020-10-24)
### Feature
* Add `add_on_changed_listener()` to `HomeeNode` to support better update handling ([`12cc3d1`](https://github.com/FreshlyBrewedCode/pymee/commit/12cc3d17ea6aa4cc3354b76f97e1833ac7b029a5))

### Fix
* Add error handling to websocket receive and send handlers ([`6e9f021`](https://github.com/FreshlyBrewedCode/pymee/commit/6e9f02191ea2d107563d962a42681d1f18f54c5b))
* Change value type in `set_value()` from `int` to `float` ([`0974bac`](https://github.com/FreshlyBrewedCode/pymee/commit/0974bacd8a78b0103d222d7357b502e6fb63e042))
* Use module relative imports ([`4f33a6f`](https://github.com/FreshlyBrewedCode/pymee/commit/4f33a6f6ae8cde8ac788e1d9e02a2d4ec0d9b666))

## v1.0.1 (2020-10-23)
### Fix
* Bump to v1.0.1 to avoid PyPI conflict ([`573e700`](https://github.com/FreshlyBrewedCode/pymee/commit/573e70054d3711196b3e39d1cc9ba80b4794a13a))

## v1.0.0 (2020-10-23)
### Feature
* Add utility methods for getting nodes and atributes by id ([`f43014c`](https://github.com/FreshlyBrewedCode/pymee/commit/f43014cb77da7a4059695663a093a4acfb3b5d02))
* Support updating/adding nodes after receiving a 'nodes' message ([`535602b`](https://github.com/FreshlyBrewedCode/pymee/commit/535602b8b43696b29f0e1e9d86bcde9e40223dbb))
* Provide async disconnected event ([`c019ef5`](https://github.com/FreshlyBrewedCode/pymee/commit/c019ef5d55306007f98ee2d0154ccee138d2cb25))
* Use coroutines for Homee callbacks ([`99296e6`](https://github.com/FreshlyBrewedCode/pymee/commit/99296e650268467df6370c034d544c10c81530a1))
* Port to websockets package ([`1b578bc`](https://github.com/FreshlyBrewedCode/pymee/commit/1b578bc166cc0d9c6238980aca1a889a2e8ddef2))

### Breaking
* Homee callbacks need to be awaitable, i.e. async functions. Handleing callbacks in the event loop should provide a better development experience since most functions in the Homee api are async now.  ([`99296e6`](https://github.com/FreshlyBrewedCode/pymee/commit/99296e650268467df6370c034d544c10c81530a1))

### Documentation
* Add badges ♥ ([`a7e3a28`](https://github.com/FreshlyBrewedCode/pymee/commit/a7e3a28e7d6d8116c893214cd6e6b24ed5758c0f))

## v0.2.0 (2020-10-23)
### Feature
* Raise unique exceptions while acquiring access token ([`edac67b`](https://github.com/FreshlyBrewedCode/pymee/commit/edac67bad668349ced6d96f8306836f884d05937))

### Documentation
* Add install instructions and bump version ([`f0208a5`](https://github.com/FreshlyBrewedCode/pymee/commit/f0208a565523e63ff0ecf976c5288ffc0d4fc71a))
* Add README ([`8701f0a`](https://github.com/FreshlyBrewedCode/pymee/commit/8701f0ad47120d8291eb5b4f4c441cc151c468b2))