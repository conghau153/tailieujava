mailto:ndangkhoa@tma.com.vn
mailto:duykhanhd@tma.com.vn
quocanhv@tma.com.vn; ‎

OmniVista Dev 1

-XX:MaxPermSize=256m -Xms128m -Xmx512m -Djava.awt.headless=true

//mongo-java-driver

C:\Program Files\MongoDB\Server\3.0\bin
mongod.exe --config D:\MongoStore\config.txt



  <build>
    <plugins>
      <plugin>
        <groupId>org.apache.tomcat.maven</groupId>
        <artifactId>tomcat7-maven-plugin</artifactId>
        <version>2.2</version>
        <configuration>
          <path>/SpringMVC</path>
          <port>8090</port>
        </configuration>
      </plugin>
    </plugins>
  </build>

  
  <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-webmvc</artifactId>
        <version>4.1.4.RELEASE</version>
    </dependency>
		

<!-- https://mvnrepository.com/artifact/jstl/jstl -->
<dependency>
    <groupId>jstl</groupId>
    <artifactId>jstl</artifactId>
    <version>1.2</version>
</dependency>

	<!-- https://mvnrepository.com/artifact/org.mongodb/mongo-java-driver -->
<dependency>
    <groupId>org.mongodb</groupId>
    <artifactId>mongo-java-driver</artifactId>
    <version>3.8.0</version>
</dependency>



public static void main(String[] args){
        MongoClient mongoClient= new MongoClient();

        MongoDatabase DB = mongoClient.getDatabase("test");
        MongoCollection collections= DB.getCollection("Emp");

        MongoCursor<Document> cursor = collections.find().iterator();
        try {
            while (cursor.hasNext()) {
                Document doc = cursor.next();
                System.out.println(doc.toJson());
            }
        } finally {
            cursor.close();
        }

    }

	
<!-- https://mvnrepository.com/artifact/com.elega9t/number-to-words -->
<dependency>
    <groupId>com.elega9t</groupId>
    <artifactId>number-to-words</artifactId>
    <version>1.0.0</version>
</dependency>

db.mycollection.insertMany( [
	    { "id" : "101", "name" : "Daniel Atlas" }, 
	    { "id" : "102", "name" : "Charlotte Neil" },
	    { "id" : "97", "name" : "tom jackmen" }
	] )

