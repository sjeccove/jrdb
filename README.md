# jrdb

자바스트립트 관계형 데이터베이스(JAVASCRIPT RELATIONAL DATABASE)

자바스트립트를 이용한 어플리케이션 개발시 관계형 데이터베이스 형태로 데이터를
저장 관리할수 있는 스크립트 라이브러이 입니다.


version 1.0.0 (wiki page 참조)

- create

  예) Sje.jrdb.create().table("db1.tbl").columns([["id",false],["column1",true],["column2",true],["column3",false],["column4",false]]).commit();

- insert

  예) Sje.jrdb.insert().into("db1.tbl").columns("id","column3","column4").values("12","23","33").commit();

- update

  예) Sje.jrdb.update().table("db1.tbl").columns("id","column2").values("value1","value2").where("column4>=11").commit();
