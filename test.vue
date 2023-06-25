interface ComponentOptions {
  inject?: ArrayInjectOptions | ObjectInjectOptions
}

type ArrayInjectOptions = string[]

type ObjectInjectOptions = {
  [key: string | symbol]:
    | string
    | symbol
    | { from?: string | symbol; default?: any }
}
