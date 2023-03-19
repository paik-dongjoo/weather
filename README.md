# weather&Diary Project

<h3> 🔥 Goal </h3>
<ul>
  <li> API를 통해 날씨 데이터를 가져오고 해당 일자에 대한 일기와 함께 기록할 수 있는 API 개발 </li>
</ul>

<h3> 📌 Point </h3>
<ul>
  <li> OpenWeatherMap API를 활용하여 설정한 나라의 날씨 데이터를 불러와 사용자가 작성한 일기와 함께 기록 </li>
  <li> Scheduler를 사용하여 매일 자정 날씨 데이터 캐싱 </li>
  <li> Swagger를 통한 API Documentation </li>
</ul>

<h3> 📚 Tech Stack </h3>

<div align="left">
	<img src="https://img.shields.io/badge/Spring%20Boot-3cb371?style=flat&logo=Spring%20Boot&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-6495ed?style=flat&logo=Java&logoColor=white" />
  <img src="https://img.shields.io/badge/JPA-9400d3?style=flat&logo=JPA&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4682b4?style=flat&logo=MySQL&logoColor=white" />
	
</div>

<h3> 📜 Final Implementation List </h3>

1. POST : /create/diary  <br>
<ul>
  <li> 사용자가 입력한 날짜와 일기데이터를 받아 데이터베이스에 저장 </li>
</ul>

2. DELETE : /delete/diary <br>
<ul>
  <li> 지정한 날짜의 일기데이터를 데이터베이스에서 삭제 </li>
  <li> 삭제하고자 하는 날짜에 저장되어 있는 일기데이터가 없을 경우 적절한 에러 메시지 반환 </li>
</ul>

3. GET : /read/diaries <br>
<ul>
  <li> 날짜 범위를 지정하여 해당 범위 내에 작성된 일기데이터 목록을 List로 반환 </li>
  <li> 너무 과거, 너무 먼 미래일 경우 별도로 설정해놓은 errorMessage 출력 </li>
</ul>

4. GET : /read/diary <br>
<ul>
  <li> 지정한 날짜의 일기데이터 목록을 List로 반환 </li>
  <li> 너무 과거, 너무 먼 미래일 경우 별도로 설정해놓은 errorMessage 출력 </li>
  <li> 읽어오고자 하는 날짜에 저장되어 있는 일기데이터가 없을 경우 적절한 에러 메시지 반환 </li>
</ul>

5. PUT : /update/diary <br>
<ul>
  <li> 선택한 날짜의 일기데이터를 수정 </li>
</ul>

![스크린샷 2023-03-20 오전 12 48 57](https://user-images.githubusercontent.com/113086103/226187834-7cdd907f-5816-4fb7-968f-f94ca3c75a31.png)
