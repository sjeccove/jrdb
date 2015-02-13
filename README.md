# jrdb

# 자바스트립트 관계형 데이터베이스(JAVASCRIPT RELATIONAL DATABASE)

# 개요

SQL DB 없이 Web Storage 중 localstorage를 이용하여 관계형 DB를 구현함.


# 사용법

version 1.0.5

- create

  예) Sje.jrdb.create().table("db1.tbl").columns([["id",false],["column1",true],["column2",true],["column3",false],["column4",false]]).commit();
  
      "db1" : database name
      "tbl" : database table name
      "id", "column1", "column2", "column3", "column4" : table column name
      "false", "true" : is null

- insert

  예) Sje.jrdb.insert().into("db1.tbl").columns("id,column3,column4").values("12,23,33").commit();

- update

  예) Sje.jrdb.update().table("db1.tbl").columns("id,column2").values("value1,value2").where("column4>=11").commit();

- select

  예) Sje.jrdb.select().from("db1.tbl").columns("id,column2").where("column4>=11").commit();
  
- delete

  예) Sje.jrdb.delete().from("db1.tbl").where("column4>=11").commit();


# 사양

웹 프라우져 (IE, Safari, Firefox, Chrome..)
