## vue3-ast-decompiler

This package all AST from the [`@vue/compiler-core`](https://github.com/vuejs/core/tree/main/packages/compiler-core)
back into a template

### Installation

```npm i vue3-ast-decompiler```

### Usage

```js
import decompile from 'vue3-ast-decompiler'

decompile(yourAstRootNode);
```

Be aware that this package heavily uses the SourceInformation from the AST, so if you transform your AST, you need to
make sure that your locations are set correctly, or you maybe get a template that will not compile
