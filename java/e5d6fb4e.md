# Converts Java Object into XML String

To serialize Java object to XML using Jackson we use XmlMapper. XmlMapper is the Jackson class that we neeed to serialization.

```
var xmlMapper = XmlMapperFactory.getXmlMapper();

var xml = xmlMapper.writeValuAsString(obj);

System.out.println(xml);
```

### References

- [Jackson xml serialization and deserialization](https://www.baeldung.com/jackson-xml-serialization-and-deserialization)
