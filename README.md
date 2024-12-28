# jtf4j - Json Transformation Framework 4 Java
A JSON Transformation Framework for Java able to work with your favorite underlaying JSON library (like Jackson, Gson, org.json and JSON-P).

Supports a high level fluent eDSL-like transformation API, as well as an implementation of the JSON Patch specification. While simple transformations can thereby be specified as JSON Patch JSON documents, you have the full capacity of Java at your disposal for transformations hard or impossible to specify as a JSON Patch document.

Independence of both the high level API as well as the JSON Patch implementation from any underlaying JSON library is achieved through a thin abstraction layer adaptable to the underlaying JSON library of your choice.

## Restrictions
- Any underlaying JSON library to be used by jtf4j needs to support a tree API
- jtf4j does not support transforming Java Beans or Records as not all underlaying JSON libraries support data binding. Java objects can therefore neither be a source for the data to be transformed, nor can they be returned from the transformation.
