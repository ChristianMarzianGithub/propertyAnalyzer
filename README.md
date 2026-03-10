# propertyAnalyzer
A webtool to analyze Spring boot properties.



Categories the analyzer should look at:
1.Configuration mistakes
"spring.jpa.hibernate.ddl-auto=create" 
=> ⚠ dangerous in production.

2.Missing required config
spring.datasource.url
=> not set.

3.Deprecated properties
spring.datasource.initialize
=> removed in newer Spring Boot versions.

4. Conflicting properties
Example:
server.port=8080
management.server.port=8080
=> may conflict depending on setup.
