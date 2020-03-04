# Best practices

## ODM Data Type Definitions

JSON schema fundamental [data types](https://json-schema.org/understanding-json-schema/reference/type.html) should be used for properties that map directly to those data types. This would be captured using the "type" quality in a property. For any property that does not map to a JSON schema fundamental date type, a reusable data type definition should be created that can then be used with the "odmType" quality for a property.

## Text Conventions
### SDF Keywords 
SDF Keywords are defined in the SDF language, for example, odmProperty. The preferred pattern for these identifiers is starting with lower case "odm" followed by camel case construction, e.g. "odmInputData".
### SDF Quality Names
SDF Quality names are extensions to the SDF language that are used to constrain definitions. Some of these are inherited from other language definitions, for example JSON Schema. The preferred construction for these identifiers is camel case, initial lower case, e.g. "widthInBits".
### Application-defined Terms
Application-defined terms are those names given to definitions in SDF. Preferred construction for these identifiers is camel case with initial upper case, e.g. "CurrentLevel".
### SDF full names
SDF full names are derived from path expressions that point to definition elements. SDF full names consist of an explicit or default namespace prefix, followed by a path expression, starting with "/" and followed by path segment names which alternate between SDF Keywords and Application-defined terms, and terminating with an SDF Quality name. For example, "zcl:/odmObject/LevelControl/odmProperty/CurrentLevel/widthInBits
SDF full names resolve to URIs
