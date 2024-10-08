<div align="center">
  <img src="https://github.com/user-attachments/assets/5bd1761a-dd3e-45c5-bdab-9e88d2fbb489" width="50%">
</div>

# ShareAlbum(앨범 공유)

## 🌐 목표
- 효율적인 개발 환경 구축: 실무에서 개발 환경 설정에 많은 시간이 소요되는 문제를 개선하기 위해, 이 프로젝트에서 Docker를 활용하여 일관된 개발 환경을 구축하고 설정 시간을 단축하고자 합니다.
- 프론트엔드 이해 필요성: 실무에서 백엔드 개발자로 일하면서도 프론트엔드의 개념을 잘 이해해야만 문제 해결과 개발 과정에서 효과적인 협업이 가능합니다. 이 프로젝트를 통해 React와 Next.js를 학습하여 프론트엔드 학습하고 프로젝트에 적용하여 실무에서 원활한 협업을 실현하고자 합니다.
- 효율적인 쿼리 작성 및 성능 최적화: 복잡한 SQL 쿼리 작성에 많은 시간이 소요되면서 비즈니스 로직에 집중하기 어려웠던 경험을 개선하고자, JPA와 QueryDSL을 학습하여 비즈니스 로직에 더 집중할 수 있도록 하였습니다. 이를 통해 간결하고 효율적인 쿼리를 작성하고, 성능 최적화 방안을 학습하고 적용하고자 합니다.

## 🛠️ Stack
**Frontend(Web)**
- **Language** : JavaScript, TypeScript
- **Library & Framework** : React, Next.Js
<br/>

**Backend**
- **Language** : Java 
- **Library & Framework** : Spring Boot
- **Database** : PostgrelSql
- **ORM** : JPA
- **Deploy**: Redis(Cache),Docker
- **Tool**: IntellJ,VSCode,Postman,JMeter
<br/>


## 🔨 프로젝트 구조
<details>
	<summary>BackEnd</summary>
  	📦 shareAlbum  <br>
	┣ 📂Backend   <br>
	┃ ┣ 📂domian  <br>
	┃ ┃ ┣ 📂album <br>
 	┃ ┃ ┣ ┃ 📂controller <br>
 	┃ ┃ ┣ ┃ 📂dto <br>
 	┃ ┃ ┣ ┃ 📂entity <br>
 	┃ ┃ ┣ ┃ 📂repository <br>
 	┃ ┃ ┣ ┃ 📂service <br>
 	┃ ┃ ┣ 📂chat <br>
 	┃ ┃ ┣ ┃ 📂controller <br>
 	┃ ┃ ┣ ┃ 📂dto <br>
 	┃ ┃ ┣ ┃ 📂entity <br>
 	┃ ┃ ┣ ┃ 📂repository <br>
 	┃ ┃ ┣ ┃ 📂service <br>
 	┃ ┃ ┣ 📂group <br>
 	┃ ┃ ┣ ┃ 📂controller <br>
 	┃ ┃ ┣ ┃ 📂dto <br>
 	┃ ┃ ┣ ┃ 📂entity <br>
 	┃ ┃ ┣ ┃ 📂repository <br>
 	┃ ┃ ┣ ┃ 📂service <br>
 	┃ ┃ ┣ 📂member <br>
 	┃ ┃ ┣ ┃ 📂controller <br>
 	┃ ┃ ┣ ┃ 📂dto <br>
 	┃ ┃ ┣ ┃ 📂entity <br>
 	┃ ┃ ┣ ┃ 📂repository <br>
 	┃ ┃ ┣ ┃ 📂service <br>
 	┃ ┃ ┣ 📂global <br>
 	┃ ┃ ┣ ┃ 📂baseEntity <br>
 	┃ ┃ ┣ ┃ 📂config <br>
 	┃ ┃ ┣ ┃ 📂jwt <br>
 	┗ ┗ ┗ ┗ 📂redis <br>
</details>
<details>
	<summary>FrontEnd</summary>
	┣ 📂frontend <br>
 	┃ ┣ 📂(member)  <br>
 	┃ ┃ ┣ 📂[nickname] <br>
 	┃ ┃ ┣ ┃ 📜layout.tsx <br>
	┃ ┃ ┣ ┗ 📜page.tsx <br>
 	┃ ┃ ┣ 📂login <br>
 	┃ ┃ ┣ ┃ 📜layout.tsx <br>
 	┃ ┃ ┣ ┗ 📜page.tsx <br>
 	┃ ┃ ┣ 📂searchResults <br>
 	┃ ┃ ┣ ┃ 📂[nickname] <br>
 	┃ ┃ ┃ ┣ ┃ 📜layout.tsx <br>
 	┃ ┃ ┃ ┣ ┗ 📜page.tsx <br>
 	┃ ┃ ┣ 📂signup <br>
 	┃ ┃ ┣ ┃ 📜page.tsx <br>
 	┃ ┃ ┣ 📂components <br>
 	┃ ┃ ┣ ┃ 📂Button <br> 
 	┃ ┃ ┃ ┣ ┗ 📜ImageButton.tsx <br>
 	┃ ┃ ┣ ┃ 📂Header <br>
 	┃ ┃ ┃ ┣ ┃ 📜Header.tsx <br>
 	┃ ┃ ┃ ┣ ┗ 📜SearchResultsHeader.tsx <br>
 	┃ ┃ ┣ ┃ 📂Modal <br>
 	┃ ┃ ┃ ┣ ┃ 📜AcceptGroupModal.tsx <br>
 	┃ ┃ ┃ ┣ ┃ 📜AddNewGroupModal.tsx <br>
 	┃ ┃ ┃ ┣ ┃ 📜AddNewPostModal.tsx <br>
 	┃ ┃ ┃ ┣ ┗ 📜InviteGroupModal.tsx <br>
 	┃ ┃ ┣ 📂context <br>
 	┃ ┃ ┃ ┗ 📜AuthContext.tsx <br>
 	┃ ┃ ┣ 📂interfaces <br>
 	┗ ┗ ┗ ┗📜MemberInfo.txt <br>  
</details>

## 데이터베이스 모델링(ERD)
<image>![스크린샷 2024-09-19 오후 4 21 59](https://github.com/user-attachments/assets/ca89026f-7369-424f-ace4-57ca08ae6523)

## 🖥️  주요 기능

### I. 회원가입 및 로그인 
  ![회원가입](https://github.com/user-attachments/assets/084f5419-04c1-46db-a39d-8b13edded9eb)
---

### II. 앨범 추가 <br> 
  ![이미지 업로드](https://github.com/user-attachments/assets/e2ff14a4-9a78-4a90-9a9b-15d1d81cd71c)
---  
### III. 그룹 추가 <br>
 ![그룹추가video-to-gif-converter](https://github.com/user-attachments/assets/cd8f3521-f33e-40d3-9045-d61c8c40633c)
---  
### IV. 회원 검색 및 그룹 초대 <br>
  ![그룹초대](https://github.com/user-attachments/assets/b7bad65d-5fd4-4281-912f-edabad9fee08)
---  

### V. 그룹 승인 및 앨범 공유 <br>
  ![초대승인](https://github.com/user-attachments/assets/539f08d7-d029-4806-b8b0-ca18e5660ef8)
---  
<br/>


## 💡 개발하며 느낀점
- 쿼리를 효율적으로 작성하는 것만으로도 성능이 크게 향상될 수 있다는 점을 깨달았습니다. 실제로 Redis와 같은 추가적인 기술을 도입하지 않아도, 쿼리 최적화만으로 성능을 충분히 개선할 수 있었습니다. 이 경험을 통해 백엔드 최적화의 중요성을 실감했습니다.
- React와 Next.js를 학습하면서 백엔드 개발자로서 프론트엔드에 대한 이해를 높일 수 있었습니다. 프론트엔드 개발 과정을 직접 경험함으로써, 백엔드와의 데이터 흐름과 API 설계의 중요성을 깨달았습니다. 이를 통해 앞으로 프론트엔드 개발자와 협력할 때, 더 원활하게 소통하고 API 규약을 명확히 정의하여 효율적인 협업을 할 수 있을 것이라고 생각합니다.
- JPA와 QueryDSL을 활용해 데이터베이스를 설계하면서, Many-to-Many 관계를 중간 테이블로 분리해 One-to-Many, Many-to-One 관계로 변환하는 과정에서 어려움을 겪었습니다. 그러나 이를 통해 객체지향적인 설계를 유지하면서 비즈니스 로직에 더욱 집중할 수 있었습니다. 이 경험은 데이터베이스 설계의 중요성과 효율적인 설계 방식이 개발 효율을 크게 향상시킬 수 있음을 깨닫게 해주었습니다.




