# TypeScript and Dojo 2

## TypeScript Roadmap Items

The following table lists TypeScript roadmap items or issues that are of interest to Dojo 2.

|Item|Version|Issue|Reason|
|----|-------|-----|------|
|Language Service Plugins|2.3|[Microsoft/TypeScript#12231](https://github.com/Microsoft/TypeScript/pull/12231)|Easier to extend TypeScript language services with additional capabilities|
|Variadic Kinds|*?*|[Microsoft/TypeScript#5453](https://github.com/Microsoft/TypeScript/issues/5453) and [Microsoft/TypeScript#9366](https://github.com/Microsoft/TypeScript/issues/9366)|Currently, there are use cases with mixins where aggregating types is necessary|
|Generic rest/spread|*?*|[Microsoft/TypeScript#10727](https://github.com/Microsoft/TypeScript/issues/10727)|While not currently tagged to a release, generic rest/spread is part of the path to variadic kinds|
|Ambient Decorators|*?*|[Microsoft/TypeScript#2900](https://github.com/Microsoft/TypeScript/issues/2900)|The ability to programatically access typing information is important|
|Conditional Decorators|*?*|[Microsoft/TypeScript#3538](https://github.com/Microsoft/TypeScript/issues/3538)|Essentially allows the equivilent of the Dojo `has()` API built into TypeScript|
|Support for project references|*?*|[Microsoft/TypeScript#3469](https://github.com/Microsoft/TypeScript/issues/3469)|Allow multiple TypeScript only projects/packages to work together without having to use transpiled code|
|Granular Targetting|*?*|[Microsoft/TypeScript#4692](https://github.com/Microsoft/TypeScript/issues/4692)|Makes it easier to target specific platforms that might have support for many ES6+ features, this requires [Microsoft/TypeScript#6974](https://github.com/Microsoft/TypeScript/issues/6974) first, which is targeted for 2.0|

## Delivered Roadmap Items

The following items have been delivered that have potential impact on Dojo 2:

|Item|Version|Issue|Reason|
|----|-------|-----|------|
|Generic type parameters|2.3|[Microsoft/TypeScript#2175](https://github.com/Microsoft/TypeScript/issues/2175)|Default values for generic type variables|
[Async iterations and Generator down levelling]|2.3|[Microsoft/TypeScript#12346](https://github.com/Microsoft/TypeScript/pull/12346)|This allows us to support non-ES6+ environments with Dojo 2, as well as ES8 for await of|
|Mixins/Traits|2.2|[Microsoft/TypeScript#311](https://github.com/Microsoft/TypeScript/issues/311)|Ability to better support mixin type functionality via [Microsoft/TypeScript#13743](https://github.com/Microsoft/TypeScript/pull/13743), [Microsoft/TypeScript#13604](https://github.com/Microsoft/TypeScript/pull/13604), [Microsoft/TypeScript#13924](https://github.com/Microsoft/TypeScript/issues/13924), and [Microsoft/TypeScript#14017](https://github.com/Microsoft/TypeScript/issues/14017)|
|`async`/`await` down levelling|2.1|[Microsoft/TypeScript#1664](https://github.com/Microsoft/TypeScript/issues/1664)|This allows us to support non-ES6+ environments with Dojo 2|
|Supporting "partial" types|2.1|[Microsoft/TypeScript#4889](https://github.com/Microsoft/TypeScript/issues/4889)|Makes it easier to say that an interface implements some items from another interface|
|ES8 Object property spread/rest|2.1|[Microsoft/TypeScript#2103](https://github.com/Microsoft/TypeScript/issues/2103)|Set to be ratified in ES8, this is available in TS2.1|
|Better Loader Plugin Support|2.0|[Microsoft/TypeScript#6615](https://github.com/Microsoft/TypeScript/issues/6615)|This allows us to properly type plugins.|
|Function `this` typing|2.0|[Microsoft/TypeScript#3694](https://github.com/Microsoft/TypeScript/issues/3694)|There are several use cases in Dojo where typing `this` within a function will improve code safety|
|Implicit index signatures|2.0|[Microsoft/TypeScript#7029](https://github.com/Microsoft/TypeScript/issues/7029)|Several of the Dojo 2 core APIs would benefit from being able to pass object literals without explicitly typing them|
|Read Only Properties|2.0|[Microsoft/TypeScript#6532](https://github.com/Microsoft/TypeScript/pull/6532)|Allows specification of interfaces that do not allow property reassignment, which can better refect runtime behaviour|
|"Native UMD"|2.0|[Microsoft/TypeScript#7125](https://github.com/Microsoft/TypeScript/issues/7125)|Solves the problem of exporting interfaces for re-importing, hopefully avoiding collisions|
|String Literal Types|1.8|[Microsoft/TypeScript#5185](https://github.com/Microsoft/TypeScript/issues/5185)|There are many instances where a string literal type will assist in making Dojo 2 more usable|
|F-Bounded Polymorphism|1.8|[Microsoft/TypeScript#5949](https://github.com/Microsoft/TypeScript/issues/5949)|The ability for generics to refer to other generics within the same argument list addresses a couple challenges in Dojo 2|
|Augmenting global type interfaces from within modules|1.8|[Microsoft/TypeScript#4166](https://github.com/Microsoft/TypeScript/issues/4166)|There are several instances when we are feature detecting within a module but need to alter the global interface as we shim in functionality|
|`this` based type guards|1.8|[Microsoft/TypeScript#5906](https://github.com/Microsoft/TypeScript/issues/5906)|Accepting a polymorphic `this` as a type guard solves some use cases in Dojo 2|


## Uncomitted Issues

The following table lists issues that are important to Dojo 2, but the TypeScript team have yet to commit to them in the roadmap:

|Item|Issue|Reason|
|----|-----|------|
|`this` as a Generic Argument|[Microsoft/TypeScript#6223](https://github.com/Microsoft/TypeScript/issues/6223)|Polymorphic `this` is a legitimate way of type guarding on extended/composed classes|
|Programmatically Modifying Types|[Microsoft/TypeScript#4490](https://github.com/Microsoft/TypeScript/issues/4490)|Revisit, with mixins being easier to achieve we may not need this|
