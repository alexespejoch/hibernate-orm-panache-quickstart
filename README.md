# hibernate-orm-panache-quickstart
 Hibernate ORM with Panache and RESTEasy

# archetype
mvn io.quarkus:quarkus-maven-plugin:1.8.1.Final:create "-DprojectGroupId=org.acme.hibernate.orm.panache" "-DprojectArtifactId=hibernate-orm-panache-quickstart" "-DclassName=org.acme.hibernate.orm.panache.FruitResource" "-Dpath=/fruits"

# database
 docker run --ulimit memlock=-1:-1 -it --rm=true --memory-swappiness=0 --name quarkus_test -e POSTGRES_USER=quarkus_test -e POSTGRES_PASSWORD=quarkus_test -e POSTGRES
_DB=quarkus_test -p 5432:5432 postgres:10.5