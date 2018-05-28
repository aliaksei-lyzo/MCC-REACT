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

5.  Describe the ways how to create components in React

        a) Using ES5 -> React.createClass method (deprecated in latest versions);
        b) Using ES6 -> Classes which extends React.Component or React.PureComponent;
        c) Using simple pure functions which take props and return markup (functional components);
        (EN)https://reactjs.org/docs/components-and-props.html

6.	What is the difference between state and props?
    
        (EN) https://reactjs.org/docs/faq-state.html

7.	Passing data from parent to children.
    
        1) Via props;
        (EN) https://reactjs.org/docs/components-and-props.html
        2) Via third-party stores (Flux, Redux, MobX);
        Flux is more like a pattern, while Redux and MobX are libraries, that are based on Flux.
        (EN) Flux - https://facebook.github.io/flux/
        (EN) Redux - https://egghead.io/courses/getting-started-with-redux
        (EN) MobX - https://egghead.io/courses/manage-complex-state-in-react-apps-with-mobx
        3) Using React 16 Context API.
        (EN) https://reactjs.org/blog/2018/03/29/react-v-16-3.html
        (EN) https://reactjs.org/docs/context.html

8.	Passing data from children to parent.
    
        1) Passing callback;
        (EN) https://reactjs.org/docs/faq-functions.html
        2) Via third-party stores (Flux, Redux, MobX);
        Flux is more like a pattern, while Redux and MobX are libraries, that are based on Flux.
        (EN) Flux - https://facebook.github.io/flux/
        (EN) Redux - https://egghead.io/courses/getting-started-with-redux
        (EN) MobX - https://egghead.io/courses/manage-complex-state-in-react-apps-with-mobx
        3) Different perversions, using NodeJS EventEmitter

9.	Lifecycle components.

        Here we must differentiate a bit between React 16 and earlier versions, since there were some major changes.
        (EN) React 16 lifecycles - https://reactjs.org/blog/2018/03/29/react-v-16-3.html;
        (EN) Lifecycles https://reactjs.org/docs/react-component.html

10.	When do we usually make AJAX calls? || Where is the best way to make AJAX calls?

        (EN) https://reactjs.org/docs/faq-ajax.html#where-in-the-component-lifecycle-should-i-make-an-ajax-call

11.	When does component rerender?

        When either state or props change, or using the forceUpdate() method.

12.	How to prevent component rerender?

        Using the shouldComponentUpdate lifecycle hook.
        (EN) https://reactjs.org/docs/optimizing-performance.html#shouldcomponentupdate-in-action

13.	If shouldComponentUpdate returns false, will the children rerender?

        By default, no, due to the reconciliation algorithm

14.	What is JSX?

        (EN) https://reactjs.org/docs/introducing-jsx.html

15.	Does browser read JSX? || What do we need to make browser understand JXS?

        No, it doesnt. We need a transpiler, e.g. Babel.

16.	Is React possible without JSX?

        (EN) https://reactjs.org/docs/faq-build.html

17.	How can we check types of React props?

        (EN) https://reactjs.org/docs/typechecking-with-proptypes.html#proptypes

18.	Forms. Controlled and uncontrolled

        (EN) https://reactjs.org/docs/forms.html

19.	Refs

        (EN) https://reactjs.org/docs/refs-and-the-dom.html
        (EN) https://reactjs.org/docs/react-api.html#reactcreateref

20.	Rendering lists. Keys

        (EN) https://reactjs.org/docs/lists-and-keys.html

21.	Reconciliation. Stack vs Fiber

        (EN) **Stack** https://reactjs.org/docs/reconciliation.html
        (EN) **Fiber** https://github.com/acdlite/react-fiber-architecture
    
22.	Data immutability

        (EN) https://www.sitepoint.com/immutability-javascript/
        (EN) https://reactjs.org/docs/optimizing-performance.html#the-power-of-not-mutating-data
        (EN) https://reactjs.org/docs/optimizing-performance.html#using-immutable-data-structures

23.	React Optimisation (use prod build, virtualize long lists, avoid reconciliation);

        (EN) https://reactjs.org/docs/optimizing-performance.html
    
24.	React.PureComponent
        
        (EN) https://reactjs.org/docs/react-api.html#reactpurecomponent
        (EN) https://reactjs.org/docs/render-props.html#be-careful-when-using-render-props-with-reactpurecomponent
        
25. Portals (React 16)
    
    (EN) https://reactjs.org/docs/portals.html
    
26. Error boundary in React 16
    
    (EN)https://reactjs.org/docs/error-boundaries.html#introducing-error-boundaries
    
27. Event handling in React

    (EN) https://reactjs.org/docs/handling-events.html
    
28. Fragments in React 16
    
    (EN) https://reactjs.org/docs/fragments.html

