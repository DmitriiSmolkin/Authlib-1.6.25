# Authlib 1.6.25 patch

Repository stores original ```authlib-1.6.25.jar``` in resources folder.

To patch, build and compile classes, you must add the original library to the local Maven storage.

```mvn install:install-file -Dfile=src/main/resources/authlib-1.6.25.jar -DgroupId=com.mojang -DartifactId=authlib -Dversion=1.6.25 -Dpackaging=jar```

After successfully adding it to the local storage you have to import dependencies from ```pom.xml``` and then build and compile patched classes.

```mvn clean install```

Compiled classes stored in ```target/classes``` directory of the current repository.