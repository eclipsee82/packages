

## Implementation
*Gradle:*
```javascript
repositories {
    maven {
        url ("https://maven.pkg.github.com/eclipsee82/packages")
        artifactUrls("https://maven.pkg.github.com/eclipsee82/packages")
        credentials {
            username = project.findProperty("gpr.user") ?: System.getenv("USERNAME")
            password = project.findProperty("gpr.key") ?: System.getenv("TOKEN")
        }
    }
}
```


## Usage




*Java Class:*
```javascript
DataGenerator dataGenerator = new DataGenerator();

String s = dataGenerator.generateText(12);
```
