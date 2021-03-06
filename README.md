# swagger-slate
Generates Slate documentation from your Swagger specification


# Building

###### Requirements
- Java 8
- Maven

```sh
git clone https://github.com/buremba/swagger-slate.git
cd swagger-slate
mvn clean install -DskipTests
```

# Running
```sh
java -jar target/client.slate-*-jar-with-dependencies.jar generate -l java,python,php -i src/main/resources/rakam-example-spec.json -o ./
```
It will output `slate.md` file in current directory, you can copy it to `slate/source/index.html.md` and Slate will update the HTML files automatically.

Currently, the supported languages are `php`, `python` `java`. `javascript` for [swagger-js](https://github.com/swagger-api/swagger-js) will be supported in first release.

# Example
[Rakam documentation](http://api.rakam.io/) is generated by swagger-slate.

# Contribution
Currently, the project is far from being mature and has many bugs & missing features.
Oauth support, `path` and `header` parameter types are not supported yet.
You are more than welcomed to contribute the project.
