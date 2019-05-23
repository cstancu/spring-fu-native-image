# Native Image instructions:

0. You need to have `native-image` on the PATH.

1. Run `cd ../../ && ./setup.sh && cd -` to build the project. You need JDK11:
```
export JAVA_HOME=${JAVA_11_HOME}
export PATH=${JAVA_HOME}/bin:${PATH}
```

2. Run `build.sh` in this directory to build the native image.

3. Run `run-native-image.sh` to run the native image created in the previous step.

4. Run `curl http://localhost:8080`. It should return `Hello world!`.
