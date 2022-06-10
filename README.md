# RestAssuredtestNgFramework

FULL INSTRUCTION IN COURCE
https://www.udemy.com/course/rest-assured-api-automation

Spotify API

https://developer.spotify.com/dashboard/login
https://developer.spotify.com/documentation/general/guides/authorization/code-flow/

Register-> Login-> get client_id and client_secret

1. Authorize
- https://accounts.spotify.com/authorize?client_id=9579ecfe28de401e9be33f5499844572&response_type=code&redirect_uri=https://google.com&scope=playlist-read-collaborative playlist-modify-public playlist-read-private playlist-modify-private&state=34fFs29kd09
-GetToken  https://accounts.spotify.com/api/token
Body:
  client_id:9579ecfe28de401e9be33f5499844572
  client_secret:5ce89bec16e941f3b8a17859cf9b5d83
  grant_type:authorization_code
  code:AQAaiOgDh9xhJMZJDzoc-esA14PfIoJ-sXobo_6YMJxlUoxeVqiXalIbN72D37e_h7egNXczfgchWalQG8NFRIsDgrpPcPbt-FCa_CbrIxLQHuybyT5A3UKVTuSP0FlLcxeqjurfV-aCMyTS9r6xkLydt8X_6q2tVwf7_4Na2bCIlk2cICh2uxHBdQ2eDUuDiTPyxQCY8Y1jDQY63J2NyoYzJrPi9IuMJlvoU2u6ZWFWylE44tc-lZuFsTHjLE4jn3LoGWn8zY5SsPfkx6LqjJ1gNijUxecJepPS
  redirect_uri:https://google.com
3. Allure command:
   mvn io.qa.meta.allure:allure-maven:serve
4. Parallel
   maven surfire plugging in pom.xml (default is: method and 10)
5. Different env run 
   mvn test -DBASE_URI="https://api.spotify.com" -DACCOUNT_BASE_URI="https://accounts.spotify.com"

