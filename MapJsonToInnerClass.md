## JsonToInnerClass

```java
A aObject = mapper.readValue(json,A.class);
aObject.setCObject(mapper.readValue(aObject.getC(),C.class));

class A {
    int a;
    String b;
    String c;
    C cObject;
}

class C {
    int d;
}
```

[https://stackoverflow.com/questions/63556308/deserialize-json-string-to-object-with-properties-which-are-strings-in-jackson]
