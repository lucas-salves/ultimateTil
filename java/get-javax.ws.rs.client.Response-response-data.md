# Getting a javax.ws.rs.client.Response response object data

Use *Response.getEntity()* method, which returns a InputStream. Then convert the InputStream result to a String.
A method to convert the InputStream to a String using _Stream Api_ example below:

```
 String result = new BufferedReader(new InputStreamReader(inputStreamToConvert))
   .lines().collect(Collectors.joining("\n"));
```
Check the reference below for more information about converting InputStream's into String:

### References
* [Stackoverflow Reference #1: How to retrieve JSON Response from a javax.ws.rs.core.Response response?](https://stackoverflow.com/questions/25196427/how-to-retrieve-json-response-from-a-javax-ws-rs-core-response-response)
* [Stackoverflow Reference #2: How do I read / convert an InputStream into a String in java?](https://stackoverflow.com/questions/309424/how-do-i-read-convert-an-inputstream-into-a-string-in-java)
