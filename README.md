# 오픈소스 과제
# 리눅스 명령어 : top, ps, jobs, kill 명령어 조사하기

# vim 에디터에서 매크로 사용방법에 대하여 조사하기 (q , @)
1. 리눅스 명령어 : top, ps, jobs, kill 명령어 조사하기

top – 실시간으로 CPU 사용률을 체크해주는 도구이다.
TOP 실행중 명령어는
a ; 메모리 사용량에 따라 정렬
b : Batch 모드 작동
c : 명령행/프로그램 이름 토글
h : 도움말
H : 스레드 토글
i : 유휴 프로세스 토글
M : 메모리 유닛 탐지
s :  보안모드 작동
S : 누적 시간 모드 토글

ps - 명령어는 현재 실행중인 프로세스 목록을 보여준다.
# -A : 모든 프로세스를 보여준다.
-N : -A 옵션과 비슷하나, ps 명령을 위해 실행한 ps 프로세스만 제외하여 보여준다. (실행을 취소한다)
-a : 세션 리더 및 터미널과 관련되지 않은 프로세스를 제외한 모든 프로세스를 보여준다.
-d : 세션 리더를 제외한 모든 프로세스를 보여준다.
-e : 커널 프로세스를 제외한 모든 프로세스를 보여준다.
T : 현 터미널에서의 모든 프로세스를 보여준다.
a : 한 터미널의 사용자 고유 프로세스를 보여준다.
r : 현재 실행중인 프로세스를 보여준다.
x : 터미널 없는 프로세스를 보여준다.
jobs - 작업이 중지된 상태, 백그라운드로 진행 중인 작업 상태, 변경 되었지만 보고되지 않은 상태 등을 표시하는 명령어다.
옵션으로는
 -l = 프로세스 그룹 ID를 state 필드 앞에 출력
 -n = 프로세스 그룹 중에 대표 프로세스 ID를 출력
 -p = 각 프로세스 ID에 대해 한 행씩 출력
 command = 지정한 명령어를 실행
kill - kill은 유닉스 계열 운영 체제에서 시스템상에서 동작하고 있는 프로세스에 간단한 메시지를 보내는 명령어이다. 기본적으로 보내는 메시지는 종료 메시지이고 프로세스에 종료하는 것을 요구한다. 
옵션으로는
-l : 시그널 리스트를 나열함.
-s : 특별히 보낼 시그널을 지정함.

2. vim 에디터에서 매크로 사용방법에 대하여 조사하기 (q , @)

 1. 명령어 모드에서 q 누른 후 매크로를 저장 알파벳을 누른다.
2. 매크로에 저장할 vim 동작 실행
3.해당 알파벳에 이후 다시 명령어 모드에서 q를 누를 때까지의 vim 동작이 매크로로 저장된다.
4. 매크로 실행은 [n]@[저장알파벳] 즉, @와 매크로가 저장된 알파벳을 누르면 된다. 
5. n을 사용해서 매크로 반복 횟수를 줄 수 있다.
