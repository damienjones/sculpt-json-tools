sculpt-json-tools
=================

JSON is great stuff. For the most part, Python native types can be trivially serialized into JSON and JSON types deserialize into native Python types. It's possible to extend the JSON encoder and decoder methods, but this is a simpler function that recursively crawls an object and returns data in a JSON-ready format, delegating field selection to nested objects.

This also has the ability to treat objects of a particular class as though they were of another class for serialization purposes; this allows you to supply serialization code for particular classes that you cannot derive from (e.g. some Java classes when running under Jython) or when the data is created of the wrong class by code you cannot change.

Special Note
------------

This is not a complete project. It's not packaged as a Python project (so you have to drop the source into your own project directly), the directory structure doesn't match the package's expectations of itself, there are no unit tests, and the only documentation is within the code itself. I don't really expect anyone else to use this code... yet. All of those things will be addressed at some point.

That said, the code _is_ being used. This started with work I did while at Caxiam (and I obtained a comprehensive license to continue with the code) so here and there are references to Caxiam that I am slowly replacing. I've done quite a bit of refactoring since then and expect to do more.

