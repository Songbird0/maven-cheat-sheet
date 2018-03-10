```xml
<properties>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
	<source-version>1.8</source-version>
	<target-version>1.8</target-version>
</properties>

<!-- ... -->

<build>
	<plugins>
		<plugin>
			<groupId>org.apache.maven.plugins</groupId>
			  <artifactId>maven-compiler-plugin</artifactId>
			  <version>3.6.1</version>
			  <configuration>
				  <source>${source-version}</source>
				  <target>${target-version}</target>
			  </configuration>
		</plugin>
	</plugins>
</build>
```
