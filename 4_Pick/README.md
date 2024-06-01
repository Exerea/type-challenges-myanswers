```
type MyPick<Type, Key extends keyof Type > = { [Property in Key]: Type[Property] };
```
<string , number>ならば

```
const example: MyType = {
    title: 42,
    completed: 1
};
```
みたいなのになる

keyofは指定したものに属しているっていう条件を付けたいってこと
