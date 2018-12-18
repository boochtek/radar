Java
====

* [Dropwizard](http://www.dropwizard.io) Java web framework
    * Probably better/simpler than Spring Boot
        * At least for APIs
    * Jetty for HTTP
    * Jersey for REST
    * Jackson for JSON
        * Still overly verbose for standard boilerplate getters/setters
    * Hibernate Validator declarative validations of user input
* [Thymeleaf](https://www.thymeleaf.org/) Java HTML templates
    * TAL - template attribute language
        * Just plain HTML with special attributes added
    * Also a new way to write plain HTML, with decoupled (in a separate file) view logic
* [Lombok](https://projectlombok.org/)
    * Annotations to reduce getter/setter boilerplate
    * Has IDE plugins for annotation processing
* [Google Auto](https://github.com/google/auto)
    * [AutoValue](https://github.com/google/auto/tree/master/value) is an alternative to Lombok
        * Provides more flexibility than Lombok, with fewer annotations, but not nearly as concise
        * Only for value object classes; no setters can be created
        * Implemented via a concrete class subclassed from an abstract class that you write
        * Have to use a builder to instantiate an object
    * AutoFactory creates JSR-330-compatible factories via annotations
    * No IDE plugins for annotation processing
* [Immutables]()
    * Another Lombok alternative
    * Only for immutable value objects
        * Implemented via a concrete class subclassed from an abstract class that you write
    * Have to use a builder to instantiate an object
    * Has IDE plugins for annotation processing
    * Automatic JSON serialization
    * Repository generation for Mongo
* [AssertJ](http://joel-costigliola.github.io/assertj/)
    * Newer alternative to Hamcrest
    * Slightly simpler syntax than Hamcrest
    * `import static org.assertj.core.api.Java6Assertions.assertThat;`
* Kotlin
    * Data classes create POJO with getters, setters, equals(), hashCode(), toString() and copy() in a single line:
        * `data class Customer(val name: String, val email: String, val company: String)`
    * Easier-to-user lambdas (with implicit `it`):
        * `val positiveNumbers = list.filter { it > 0 }`
    * Easy singletons:
        * `object ThisIsASingleton {}`
    * Optional semi-colons
    * Improved type signature syntax:
        * `var output: String`
        * `fun main(args: Array<String>) {}`
    * Create object Python-style (without the `new`)
    * String interpolation:
        * `println("Hello, $name")`
    * Explicit nullable types; protection from NullPointerException
        * `val name: String? = null`
        * `println(name.length())      // Compilation error`
