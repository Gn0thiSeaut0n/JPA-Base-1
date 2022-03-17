# JPA-Base-1

JPA 완전 기초 연습

H2 Database의 버전에 따라 jdbc url이 다름

기본적으로 jdbc:h2:mem:test 또는 jdbc:h2:mem:testdb

이런식으로 잡혀있는데 PC의 h2 콘솔로 접속하면 Intellij에서 h2 데이터를 조작할 때 조회가 되지 않거나 하는 현상 발생

예제들을 보면 jdbc:h2:tcp://localhost/~/test 이런식으로 url이 잡혀있는데 이렇게 사용해야 양쪽에서 데이터가 조회되거나 사용가능


수정 방법

해당 위치에서 메모장 파일을 만들고 test.mv.db로 파일명 수정(내용은 넣지 않는다)
- ex) C:\Users\hncis에 test.mv.db 파일 생성

웹에서 localhost:8082 쳐서 h2 database 콘솔창에 진입

url을 jdbc:h2:tcp://localhost/~/test로 치고 연결 시도

