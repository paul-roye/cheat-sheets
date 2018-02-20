# Analysis parameters

 
 | Parameter  | Description | Default value   | 
 |---|---|---|
 | sonar.host.url  | Server URL  | http://localhost:9000   | 
 | sonar.project.key  | The project key that is unique for each project.|  When using maven it's set to <br/> <groupId\>:<artifactId\>   | 
 | sonar.login  | The login of a SonarQube user with Execute Analysis permission.  |   | 
 | sonar.password  | The password that goes with sonar.login.  |   | 
 | sonar.language  | Set the language of the source code to analyse  | If not set multi-language analysis will be triggered  | 
 


# Tools

- Sonarlint : 
  <ul>
    <li>Allows  to fix issues on the fly and when code changes</li>
    <li>Available as a plugin for IDE</li>
    <li>[sonarlint web site](https://www.sonarlint.org/)</li>
  </ul>
- EclEmma : 
  <ul>
    <li>Allows to check coverage code by unit tests. It's based on JaCoCo library </li>
    <li>Available as a plugin for Eclipse IDE</li>
    <li>[EclEmma web site](http://www.eclemma.org/)</li>
  </ul>
- Jscpd : 
  <ul>
    <li>Allows to detect copy/paste code </li>
    <li>[Jscpd web site](https://github.com/kucherenko/jscpd)</li>
  </ul>