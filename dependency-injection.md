You don't need a DI container, unless you absolutely need cross cutting concerns and proxy generation for your components

Most small to medium projects can go a long way by "wiring" the classes just with code, instead of declaring beans and injecting them all over the place

Even if you strife for proxies - most of annotations can be replace with a manual method call that will do the same magic

Benefits of not having a DI container are:
 * Fast startup
 * Smaller application footprint
 * Type safety auto of the box for statically typed languages
 * Easier to navigate and read, no need for special introspecting tools and IDE/Editor plugins
