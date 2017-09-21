---
layout: post
title : MySQL Query 확인 방법
category : mysql
tags : [mysql, prompt]
---
## 개요
- MySQL에서 실행되는 전체 쿼리를 확인하고자 할 때 사용
- Hibernate 2차캐쉬를 사용하여 캐쉬에서 결과를 받을 경우, MySQL 쿼리가 호출되지 않았는지 확인하고자 할 때 로그 확인


## 작업
- MySQL 서버에 프롬프트에서 아래와 같이 실행
```mysql
mysql> set global general_log=on;
```

- 로그파일명(general_log_file)을 확인하는 방법
```mysql
mysql> show variables like 'general%';
```

