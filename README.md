

## Implementation
*Gradle:*
```javascript
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/eclipsee82/packages")
    }
}
```


## Usage




*Java Class:*
```javascript
DataGenerator dataGenerator = new DataGenerator();

String s = dataGenerator.generateText(12);
```