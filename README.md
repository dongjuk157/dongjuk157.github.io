# 포트폴리오 사이트 구축

### 구현할 페이지

1. index.html
   - 첫 페이지
2. introduce
   - 소개
   - 무엇을 하고싶은지 (future)
   - 어떤 생각을 가지고 있는지 (future)
   - 뭐 해먹고 살지 (future)
3. history
   - 약력(출생, 학력 등 연대 순으로 기술)
4. projects
   - 대학교 전공이나 동아리, 혼자 했던 프로젝트들 정리
   - 기술별로 정리? 
5. contact
   - phone number
   - mail
   - instagram, github, linkedin



### 개발 일지

2021-02-08

- Bootstrap을 사용해서 빠르게 index.html을 만들었다.
- navbar와 carousel을 가져왔다.
- navbar의 맨 왼쪽에 위치하는 이미지를 가져오고 싶은데 뭘 가져와야할지 모르겠다.
- Font awesome에서 이모티콘 몇개도 가져와서 사용해봤다.
- contact도 만드려했는데 fa에서 가져온 이모티콘들의 width 사이즈가 안맞는다.
- 따로 칸을 가운데 정렬좀 시켜야겠다.
- 대충 어떻게만들지는 구상했는데 디자인이 가장 어려운거같다.
- 나머지 페이지는 비어있는 페이지로 navbar만 복사해서 붙여넣었다.



2021-02-09

- History를 timeline으로 구현하려했지만 scroll animation을 너무 넣고싶었다. 

- 아직 js를 배우지 않아서 막 가져다 쓰기에 괜히 불안하니 공부부터 하고 나중에 구현해야지.
  
  - 설에 시간을 내어 생활코딩이라도 보고 기본이라도 잡아야겠다.
  
- 지난번에 못했던 contact 페이지를 만들었다.

- 어제 만들었던 페이지와 큰차이가 없고 그리드를 사용해서 칸을 나눠 사용했다.

- 아이콘은 어제와 마찬가지로 font awesome 에서 가져왔다.

- 상당히 심플하게 만들었는데도 배치가 매우 어려웠다.

- 마진, 패딩을 조금씩 설정하고 그리드로 offset을 조정해가면서 내눈에 보기 편하게 만들었다.
  
  - index.html 제목도 패딩 조금 설정했다.
  - 올리고보니 패딩좀 줄여야겠다. 아래 짤려서 스크롤바 생기네
  
- bootstrap이 반응형이라 viewport 크기에 따라 계속 바뀌는데 min width를 정하고 싶다.

  

2021-02-10

- https://colorhunt.co/



2021-02-11

- navbar의 sticky-top 해제
  - 굳이 상단 고정 안해도 될것같다.
  - 옆에 sticky로 따라다니는 메뉴를 만드는게 나을듯
- 탭이 너무 많아보임
  - navbar의 img_maing 삭제
  - Future 삭제(introduce와병합)
  - Main이랑 introduce랑 합칠지 고민중(아직은 삭제안함)
- Projects 탭 작성
  - card와 modal를 사용할 것이다.
  - card로 간단하게 보여주고, 클릭했을때 modal로 자세한 내용을 기술한다.
  - 카드에 들어가는 이미지들 크기가 너무 중구난방이어서 card 크기의 50 퍼센트를 쪼개고 그안에 `object-fit:contain`을 사용해서 넣었다.
  - 그 아래 들어가는 글들은 최대 4줄(제목1줄, 내용3줄)정도가 가장 적합한것같다.
  - 카드 높이들은 어떻게 맞춰야하는지 모르겠다. 같은 줄끼리는 맞춰지는데 다른 줄끼리는 높이가 같지 않아서 조금 불편하다.
  - 카드를 눌렀을때 modal을 사용할지 page를 몇개 더 만들지 갑자기 고민된다..
- navbar collapse 적용, 색상 적용
- introduce 조금 추가
- history도 삭제?
  - 삭제 안함(21-02-14)



2021-02-12

- project에 modal 추가
  - modal을 추가하고 싶은 태그에 `data-bs-toggle="modal" data-bs-target="#exampleModal"`이렇게 추가하고 target과 같은 id의 모달을 만들면 된다.
  - button 클릭 말고 card 자체 클릭하면 뜬다.
  - 내용은 사진들이 없어서 그냥 ul,li 태그로 몇개 적었다.



2021-02-13

- 아무것도 하기 싫어서 놀았다.
- 주말인데 좀 쉴 수도 있잖아



2021-02-14

- history 제작
  - `history.html`, `css/hitsory_style.css`
  - https://bootstrapious.com/p/timeline 
  - 위 주소에 나온 코드를 사용했고 색깔 몇개 바꾸고, 적용 안되는거 몇개 바꿈(`ml`을 `me`등으로 바꿈)
- introduce 제작
  - 길게~길게~ 작성
- contact 수정
  - 가운데로 옮김
  - 반응형 ㅇㅋ



### 사용한 기술

HTML, CSS, Bootstrap

키보드와 마우스를 이용한 복사 붙여넣기 기술

시간을 갈아넣는 기술