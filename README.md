# pieimg
Draw pie chart by Go with mermaid-cli

## Prerequisites

- [Go](https://go.dev/) 1.17 or later
- [Node.js](https://nodejs.org/) (required by mermaid-cli)
- [mermaid-js/mermaid-cli](https://github.com/mermaid-js/mermaid-cli)

Install mermaid-cli with:
```
npm install -g @mermaid-js/mermaid-cli
```

## Usage

Edit `sample.mmd` to describe your pie chart in [Mermaid syntax](https://mermaid-js.github.io/mermaid/#/pie), then run:

```
go run main.go
```

The chart is rendered and saved as `sample.png`.

### Options

| Flag           | Description                        |
| -------------- | ---------------------------------- |
| `-dark`        | Render with dark theme             |
| `-transparent` | Use a transparent background       |

```
go run main.go -dark -transparent
```

## Example

**Input** (`sample.mmd`):
```
pie title Today's plan
    "Sleeping" : 6
    "Coding" : 1
    "Play with Daughter" : 3
    "Zone out" : 14
```

**Output** (`sample.png`):

![sample](sample.png)

## References
* [mermaid](https://mermaid-js.github.io/mermaid/#/)
* [mermaid-js/mermaid-cli](https://github.com/mermaid-js/mermaid-cli)