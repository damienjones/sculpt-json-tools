sculpt-json-tools
=================

JSON is great stuff. For the most part, Python native types can be trivially serialized into JSON and JSON types deserialize into native Python types. It's possible to extend the JSON encoder and decoder methods, but this is a simpler function that recursively crawls an object and returns data in a JSON-ready format, delegating field selection to nested objects.

This also has the ability to treat objects of a particular class as though they were of another class for serialization purposes; this allows you to supply serialization code for particular classes that you cannot derive from (e.g. some Java classes when running under Jython) or when the data is created of the wrong class by code you cannot change.
