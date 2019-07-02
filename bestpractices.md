Best practices

ODM Data Type Definitions:
JSON fundamental data types should be used for properties that map directly to those data types. This would be captured using the "type" quality in a property. For any property that does not map to a JSON fundamental date type, a reusable data type definition should be created that can then be used with the "odmType" quality for a property.

