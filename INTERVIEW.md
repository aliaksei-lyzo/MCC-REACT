# What you need to know for basic React interview, Q&A.

1.	What is React?
    React is a component based library for building user interfaces. There is a holywar about whether React is a library
    or a framework.

    IMHO (use with caution) Officially it is a library, but IMHO it is already not, because in some way it defines
    the way we structure our application, but it is not a framework, as it doesn't provide that much tools and is not
    that strict as real frameworks. It is something between a library and a framework.

2.	Could you compare MVC and React? Angular and React?
    Unlike Angular, which is MVC, React doesn't provide full out-of-the-box frame for the whole web-application.
    Instead, React focuses only on creating views (V from MVC), leaving the business logic and code structure
    decisions to the team or a developer.
    (EN): https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d
    (RU): https://habr.com/post/338068/
    (EN): https://medium.com/unicorn-supplies/angular-vs-react-vs-vue-a-2017-comparison-c5c52d620176

3.	What are the killer features of React? || What is JSX? || What is VirtualDOM?
    JSX, VirtualDOM.
    JSX(EN): https://reactjs.org/docs/introducing-jsx.html
    Virtual DOM(EN): https://reactjs.org/docs/faq-internals.html#what-is-the-virtual-dom
    Advanced knowledge about VirtualDom(EN): https://www.youtube.com/watch?v=xsKYAa1ZXpQ

4.	What are two main types of components?
    Basically, there are two types of components - state(-ful) and stateless || smart and dumb || container and view etc.
    (RU) https://code.tutsplus.com/ru/tutorials/stateful-vs-stateless-functional-components-in-react--cms-29541

5.  Describe the ways how to create components in React.
    a) Using ES5 -> React.createClass method (deprecated in latest versions);
    b) Using ES6 -> Classes which extends React.Component or React.PureComponent;
    c) Using simple pure functions which take props and return markup (functional components);

    (EN)https://reactjs.org/docs/components-and-props.html

5.	What is the difference between state and props?
    Both state and props represent the information, basing on which the view depends. Both the change of state
    and props causes components to rerender. The state represents the inner status of the component,
    while the props come from outside.

6.	Passing data from parent to children.
    1) Via props

7.	От дочернего к родителям.
8.	Жизненные циклы компонента.
9.	В каком обычно ставят AJAX запрос?
10.	Когда происходит перерисовка компонента?
11.	Как предотвратить перерисовку компонента?
12.	Если shouldComponentUpdate возвращает false, то будут ли перерисованы дочерние?
13.	Что такое JSX?
14.	Читается ли JSX браузером? Что для этого нужно?
15.	React без JSX?
16.	JS слабо типизирован. Можно ли организовать валидацию props, не прибегая к написанию функций-валидаторов? (prop-types, Flow);
17.	Формы. Контролируемые и контролируемые формы.
18.	Refs. Refs у stateless components.
19.	Отрисовка списков. Keys.
20.	Reconciliation*. Stack vs Fiber
21.	Data immutability
22.	React Optimisation (use prod build, virtualize long lists, avoid reconciliation);
23.	React.PureComponent;
