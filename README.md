# eGov-cms
- 유저
	1. 이메일,비밀번호, 이름 
	2. 이메일 중복방지
	3. 이메일 인증 
	4. 비밀번호 변경, 회원탈퇴 
	5. 비밀번호 찾기 이메일 
	6. 관리자 계정
- 게시판 관리 (관리자 계정일 경우에만 사이드바로 출력)
    - 생성
		1. 카테고리이름, 설명, 타입(공지사항, 자유게시판, 겔러리), 파일 허용여부
		2. 이름 중복 방지
    - 조회
		1. 카테고리별 게시글 조회
		2. 전체선택, 일부선택 selectbox로 삭제
		3. 카테고리 삭제시 게시글,게시글에 첨부된 댓글,파일 삭제 
- 게시글
    - 생성
		1. 제목, 내용, 작성자(유저 정보가져와 자동입력), 작성시간, 파일
		2. 공지사항 카테고리는 관리자 계정만 글 작성 할 수 있도록
    - 조회
		1. 카테고리, 제목, 내용, 작성자, 파일 보여주기
		2. 댓글 출력 및 작성
		3. 게시글 삭제시 파일, 댓글 삭제 
    - 검색
		1. 타입별 검색 
		2. 검색시 페이징처리 
- 파일
	1. 년/월/일 별로 파일 별도 분리 저장
	2. 파일명 중복방지로 uuid 붙여서 저장
	3. 다운로드시 uuid는 제거하고 원래 파일명으로 다운로드
- 댓글
	1. 작성자(유저 정보가져와 자동입력), 작성시간, 내용
	2. 댓글 별도 삭제
	3. 작성자, 관리자만 삭제
	4. 별도의 db 구성하되 boardNo으로 불러오고 저장 
