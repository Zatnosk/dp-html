# Declarative Programming in HTML
This is an experiment investigating syntax and expressability in declarative programming. 

## click-action
```html
<button onclick="my-action">
  <action id="my-action">
    <attribute target="#my-element" name="class" add="my-class">
  </action>
</button>
```

## conditional
```html
<if condition="$bool1 or ($bool2 and $bool3)">
  <p>This paragraph is shown/included in the document, if and only if the condition attribute evaluates to true.
</if>
```

## fetching external resources
```html
<fetch href="https://example.com/resource.html" mode="cors" method="get">
  <header name="Authorization">Bearer <value>token</value></header>
</fetch>
```

```html
<fetch href="/api/endpoint" method="post">
  <header name="Authorization">Bearer <value>token</value></header>
  <body>
    key1: value_a
    key2: value_b
  </body>
</fetch>
```
