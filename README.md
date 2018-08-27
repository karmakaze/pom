# pom
A maven dependency adder/remover/updater

## Building

- mvn clean package

## Running

- java -jar target/pom-1.0-SNAPSHOT.jar

## Packing as a single executable file (does not include java runtime)

- mvn clean package
- cat src/pom.sh target/pom-1.0-SNAPSHOT.jar >pom
- chmod a+x pom

Note that `pom.sh` just contains `exec java -jar $0`$@
