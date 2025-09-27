# hello-github-maven

none of your damn business:  

WjJod1h6QkJlRTFtZGpsd1ZGWldTSGRQTm10aGVUUlVNVlJ6Tm5kTGIzSTVkak40VEc5dWRRPT0=

mvn deploy : to publish your artifact  

to consume the artifact, add a settings.xml to your maven local directory(.m2) inside your ${user.home}.  
a settings_example.xml is given for your reference. add this to your pom.xml  

```
    <dependencies>
        <dependency>
            <groupId>com.uglyeagle</groupId>
            <artifactId>hello-github-maven</artifactId>
            <version>1.0.1</version>
        </dependency>
    </dependencies>
    
    <repositories>
        <repository>
            <id>github</id>
            <url>https://maven.pkg.github.com/Suraj-Mohapatra/hello-github-maven</url>
        </repository>
    </repositories>
```

also you can configure nexus or artifactory as a mirror to maven central. unused settings are commented out in settings_examole.xml.  

note** process is same for all JVM langauges as this is maven specific.  

note** you may also use the GitHub Actions workflow 'Publish Java Package with Maven' to automatically build and publish a project to GitHub Packages whenever you create a release. For this I have created another project, url : https://github.com/Suraj-Mohapatra/maven-github-workflows  

I may add remaining information whenever I feel like it; meanwhile, do some homework contribute more than complain.
