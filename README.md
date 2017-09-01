# 학과 게시판 새 글 알림 시스템 (v 0.0.2)
### # 학과 게시판에 새 글이 게시되었을 때 모바일 앱으로 푸쉬 알림을 보내는 서버 시스템입니다.
### # 시스템은 주기적으로 게시판을 파싱하여 새 글이 발견됐을 때, 푸쉬 알림을 전송합니다.
### # 사용자는 알림 받기 원하는 게시판을 추가/삭제하여 시스템으로부터 알림 기능을 제공받습니다. (Client : android device)

<br>

## 시스템 흐름
<pre><code>1. 시스템 시작
2. 백업 파일 로딩 : 게시판이 저장되어 있는 파일 로딩
3. 메모리 이동 : 효율적인 작업을 위해 파일 데이터를 메모리로 복사
4. 새 글 검사 알고리즘 시작
(4-1) 메모리에 존재하는 모든 게시판을 파싱
(4-2) 새 글 발견시 해당 게시판을 추가한 사용자 토큰 조회
(4-3) 푸쉬 알림 전송
(4-4) 새 글 검사 알고리즘 반복
</code></pre>

<br>

## 개발환경
### # Tools
<pre><code>- IDE : STS(Spring Boot)
- DB : MySQL
</code></pre>
### # Dependencies
<pre><code>- JSoup
- MyBatis
</code></pre>

<br>

## 추후 수정사항 (0.0.2 -> 0.0.3)
### # Server Side
<pre><code>- 서버 구동 중 발생되는 json 오류 수정
</code></pre>
