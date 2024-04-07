# `ServerOptionsSection`

Section of options.

## Syntax

```ts
type ServerOptionsSection = {
    type: string
    title: Text | (string & {})
    icon?: Icon
    options: ServerOption[]
}

type ServerOption =
    | ServerTextOption
    | ServerSliderOption
    | ServerToggleOption
    | ServerSelectOption
    | ServerMultiOption

type ServerTextOption = {
    query: string
    name: Text | (string & {})
    type: 'text'
    placeholder: Text | (string & {})
}

type ServerSliderOption = {
    query: string
    name: Text | (string & {})
    type: 'slider'
    def: number
    min: number
    max: number
    step: number
    unit?: Text | (string & {})
}

type ServerToggleOption = {
    query: string
    name: Text | (string & {})
    type: 'toggle'
    def: 0 | 1
}

type ServerSelectOption = {
    query: string
    name: Text | (string & {})
    type: 'select'
    def: number
    values: (Text | (string & {}))[]
}

type ServerMultiOption = {
    query: string
    name: Text | (string & {})
    type: 'multi'
    defs: boolean[]
    values: (Text | (string & {}))[]
}
```
