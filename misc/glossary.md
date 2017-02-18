# Glossary

Glossary of terms used within the **Honey** framework.

### 1. `style descriptor` or `descriptor`

A style descriptor, very simply, is a description of a particular style or group of styles. This description is written in `.json`, which is an agnostic way of defining a specification. In this way, we can use these abstracted descriptions to construct anything we want, be it style assets, CSS or any preprocessor defined syntax, or even a documentation website.

###### 1.1 `descriptor type` or `type`

This is an identifier for different types of descriptors, defined as a string. See a [full list](https://github.com/honeyframework/honey/wiki/Style-Description-Specification#list-of-descriptor-types).

### 1. `style description` or `description`

A collective of `descriptors` is referred to as a `style description`.

###### 1.1 `expected definition`

### 1. `comb`

### 1. `dipper`

A `dipper` is essentially a function, which accepts a `description` object, consumes it in some way, outputting the relevant files, and then when it's done return the very same `description`, unchanged. This allows for `dippers` to be stacked on each other, each one performing a specific action without interfering with the other, and being able to worry about it's own use case of the `description`.
