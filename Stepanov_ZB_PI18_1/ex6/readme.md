# Лабоаторная работа №6. Props, State и события 

### Контрольные вопросы

1. В чем отличие Props от State?

> *После рендера, есть существенное различие: props передаётся в компонент (служат как параметры функции), в то время как state находится внутри компонента (по аналогии с переменными, которые объявлены внутри функции)*

2. В чем разница между обработкой событий в React и элементов DOM с помощью обычного JavaScript 

> *Есть несколько синтаксических отличий:*
> * *События React именованы с использованием верблюжьей нотации вместо нижнего регистра.*
> * *С помощью JSX в качестве обработчика события вы передаете функцию, а не строку*

### Дополнительные задания

> *Добавьте другие контролы к кнопке на страницу html*

#### Содержимое кнопки меняет значение, при нажатии:
```
const moyai = "https://i.pinimg.com/originals/16/9d/b7/169db784351539f990e7c770720cf075.png";
...
let changeLabel = (this.state.label === "Нажми") ? <img src={moyai}></img> : "Нажми";
this.setState({ class: className , label: changeLabel });
```