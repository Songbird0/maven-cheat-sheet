```xml
<properties>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
	<source-version>1.8</source-version>
	<doc-level>protected</doc-level>
	<package-type>jar</package-type>
</properties>

<!-- ... -->

<build>
  <plugins>
	  <plugin>
		  <groupId>org.apache.maven.plugins</groupId>
		  <artifactId>maven-javadoc-plugin</artifactId>
		  <version>2.10.4</version>
		  <executions>
			  <execution>
				  <id>attach-javadocs</id>
				  <goals>
					  <goal>${package-type}</goal>
				  </goals>
				  <configuration>
					  <show>${doc-level}</show>
				  </configuration>
			  </execution>
		  </executions>
		  <configuration>
			  <charset>${project.build.sourceEncoding}</charset>
			  <docencoding>${project.build.sourceEncoding}</docencoding>
			  <docfilessubdirs>true</docfilessubdirs>
			  <show>${doc-level}</show>
			  <source>${source-version}</source>
		  </configuration>
	  </plugin>
  </plugins>
</build>
```
