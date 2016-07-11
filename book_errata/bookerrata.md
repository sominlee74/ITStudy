# 오탈자 정리

## 나의 첫 아두이노 프로젝트

* [해당 도서의 오탈자 안내 페이지@인사이트북](http://www.insightbook.co.kr/books/making-insight/%EB%82%98%EC%9D%98-%EC%B2%AB-%EC%95%84%EB%91%90%EC%9D%B4%EB%85%B8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%EC%98%A4%ED%83%88%EC%9E%90-%ED%8E%98%EC%9D%B4%EC%A7%80#respond)

### 내가 찾은 오탈자 및 오류
1.  p18, line3~6: Long과 Unsighed Long의 범위가 틀렸음
	1.  long: -2,147,483,648 to 2,147,483,647  (ref:https://www.arduino.cc/en/Reference/Long )
	2.  unsinged long: 0 to 4,294,967,295 (2^32-1) (ref: https://www.arduino.cc/en/Reference/UnsignedLong )
2.  p18, line 14. C/C++ integer array 예제오류
	
	책의 내용
	
	    int values[2];
	    int values[0] = 42;
	    int values[1] = -42;
	    int more_values[] = { 42, -42 };
	    int first = more_values[0];
	
	수정내용
	
	    int values[2];
	    values[0] = 42;  // 앞에서 이미 선언되었으므로 다시 int로 형을 선언하면 에러남
	    values[1] = -42;
	    int more_values[] = { 42, -42 };
	    int first = more_values[0];




