- run <code>app-config</code> and <code>discovery</code> servers
- run <code>breaker-hystrix</code> application  
<code>mvn spring-boot:run</code>

## Test Application
- go to hystrix dashboard <code>http://localhost:8088/hystrix</code>
  - paste <code>http://localhost:8087/hystrix.stream </code> and enter
  - this would monitor the <code>breaker-hystrix</code> application
- open new tab and hit end-point of <code>breaker-hystrix</code> application 
  - <code>http://localhost:8087/book-service-instance</code>
- monitor former tab as you refresh second tab