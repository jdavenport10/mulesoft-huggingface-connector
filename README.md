None of this is clearly laid out in documentation so just in case. 

1. This project will only compile with Java 8, which is no longer available through Oracle. Install this using brew and adoptopenjdk

2. You need to make sure your Java Version and Maven Java Version align properly. Run `java -version` and `mvn -version` to make sure both are pointing to your newly installed adoptopenjdk.
    - If they aren't, make sure that /usr/local/bin/java is simlinked to /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home/bin/java and JAVA_HOME is set to /Library/Java/JavaVirtualMachines/adoptopenjdk-8.jdk/Contents/Home