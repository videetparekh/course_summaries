# LESS

*LESS* is a *CSS* preprocessor with a twist. It follows regular *CSS* syntax with certain addition features like `variables`, `operations`, `nesting`, `mixins` and `scoping`.

It makes regular CSS code more reusable and the application itself scalable while maintaining syntactical simplicity and ease-of-use. *LESS* is run within Node and can be used in the command line via npm, within third party converters as well as the official *LESS* online editor.

### Variables

Many values are reused over and over in *CSS* code. Variables allow us to store these values externally and call them as and when required. This can be done in the following manner:

```LESS
@variableName: variable_value;

@color: #fffeee;
@stringVal: "This is an example";
```



### Import

Import statements may be used to reference external variables and mixins to further improve *LESS* development.

```LESS
@import "../tidal-wave.less";
```



### Extend

Extend is *LESS* subclass which merges the selector it is put on with ones that match it's reference.

```LESS
nav ul {
  &:extend(.inline);
  background: blue;
}
.inline {
  color: red;
}
```



### Mixins

Mixins are *LESS* functions that allow mixing and matching of multiple classes. Mixins can also be functions. They provide a template for performing a certain styling operation, and make code reusable. An example of a mixin is: 

```LESS
.border-top-radius(@radius) {
    border-top-right-radius: @radius;
    border-top-left-radius: @radius;
}

div {
    .border-top-radius(125px);
    background: rgb(255, 255, 255);
    display: inline-block;
    padding: 50px;
}
```



### Nesting

Nesting allows inheritance of children. It reduces the amount of code one has to write and but it is extremely powerful.

```LESS
article {
    a {
        color: green;
    }
    p {
        color: black;
        a {
            color:blue;
        }
    }
}
```



### Operations

Operations allow one to perform mathematical calculations and operations within *LESS*. 

```LESS
@container-tablet : (( 720px + @grid-gutter-width));
```

