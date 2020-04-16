# @shadoll/viola
> element component chalk theme.


## Installation
```shell
npm i @shadoll/viola -S
```

## Usage

отличие от обычного пакета

- объявляете переменные верхнего класса
```scss
// sass | scss

$core-class: fk-tomato;

// mix
$namespace: $core-class + ' .el';
$namespace2: $core-class + '.el';

// optional
$--color-primary: violet;
```
обратить внимание на переменную `$core-class` - название класса (без точки)
`$namespace` и `$namespace2` - служебные (нужны для sass @mixin)

- после переменных импортируете пакет на верхнем уровне
```scss
// sass | scss
@import "~@shadoll/viola/src";
```

---

если не будете использовать эти особенности - не рекомендую использовать этот 
пакет взамен обычного `element-theme-chalk` , так как тут он немного "раздувается".

ниже документация от родного пакета `element-theme-chalk`

Use Sass import
```css
@import '@shadoll/viola';
```

Or Use webpack
```javascript
import '@shadoll/viola';
```

Or
```html
<link rel="stylesheet" href="path/to/node_modules/@shadoll/viola/lib/index.css">
```

##  Import on demand
```javascript
import '@shadoll/viola/lib/input.css';
import '@shadoll/viola/lib/select.css';

// ...
```
