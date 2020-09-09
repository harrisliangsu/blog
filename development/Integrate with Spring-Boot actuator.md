### Requirements
* Spring-Boot: 2.1.7.RELEASE
* Maven: latest
* Java: JDK8


### Add dependency

#### Actuator
```xml
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-actuator</artifactId>
        <version>2.1.7.RELEASE</version>
    </dependency>
```

#### Build-info
```xml
    <plugin>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-maven-plugin</artifactId>
        <executions>
            <execution>
                <goals>
                    <goal>build-info</goal>
                </goals>
            </execution>
        </executions>
    </plugin>
```

#### Git-info
```xml
    <plugin>
        <groupId>pl.project13.maven</groupId>
        <artifactId>git-commit-id-plugin</artifactId>
        <version>4.0.0</version>
        <executions>
            <execution>
                <id>get-the-git-infos</id>
                <goals>
                    <goal>revision</goal>
                </goals>
                <phase>initialize</phase>
            </execution>
        </executions>
        <configuration>
            <generateGitPropertiesFile>true</generateGitPropertiesFile>
            <generateGitPropertiesFilename>${project.build.outputDirectory}/git.properties</generateGitPropertiesFilename>
            <includeOnlyProperties>
                <includeOnlyProperty>^git.build.*$</includeOnlyProperty>
                <includeOnlyProperty>^git.commit.id.*$</includeOnlyProperty>
                <includeOnlyProperty>^git.branch$</includeOnlyProperty>
            </includeOnlyProperties>
        </configuration>
    </plugin>
```

### Config
```properties
# Show the all git information in api /info
management.info.git.mode=full
```