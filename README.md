

## Implementation
*Gradle:*
```javascript
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/eclipsee82/packages")
    }
}


dependencies {
    implementation ('org.example:test-package:1.0.0')
}
```


*Maven:*
```javascript
<repositories>
        <repository>
            <id>github-packages</id>
            <url>https://maven.pkg.github.com/eclipsee82/packages</url>
            <snapshots>
                <enabled>true</enabled>
            </snapshots>
            <releases>
                <enabled>true</enabled>
            </releases>
            <credentials>
                <username>${env.USERNAME}</username>
                <password>${env.TOKEN}</password>
            </credentials>
        </repository>
    </repositories>


    <dependencies>
        <dependency>
            <groupId>org.example</groupId>
            <artifactId>test-package</artifactId>
            <version>1.0.0</version>
        </dependency>
    </dependencies>
```



## Usage
*Java Class:*
```javascript
DataGenerator dataGenerator = new DataGenerator();

String s = dataGenerator.generateText(12);
```
