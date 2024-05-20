# opensw
리눅스 명형어 top, ps, jobs, kill 명령어에 대한 조사

## top
top 명령어의 주요 기능
1. 실시간 시스템 모니터링
- cpu, 메모리, 스왑 사용량, 시스템 업타임 등 시스템의 상태를 실시간으로 표시
2. 프로세스 정보
- 현재 실행하고 있는 모든 프로세스 목록을 표시, 각 프로세스의 PID, 사용자, CPU, 메모리 사용률, 실행 시간, 명령어 등을 보여줌
3. 정렬 및 필터링
- 기본적으로 CPU 사용률을 기준으로 프로세스 정렬, but 메모리 사용량, PID 등 다양한 기준으로 정렬 가능
- 특정 사용자의 프로세스만을 볼 수 있고 특정 조건에 맞는 프로세스를 필터링 가능

### top 명령어
<img width="851" alt="image" src="https://github.com/ssswoowoook/opensw/assets/170293211/bde5bd69-6104-4bf8-9652-3dce83df8abc">

top 명령어의 주요 인터페이스 요소
시스템 시간, 업타임, 사용자 세션 수, 로드 평균, 작업 상태, CPU 상태, 메모리 사용량, 스왑 사용량

프로세스 목록
PID, 사용자 이름, 우선 순위, NICE 값, 가상 메모리 사용량(VIRT), 물리 메모리 사용량(RES), 공유 메모리 사용량(SHR), CPU 사용률(%CPU), 메모리 사용률(%MEM), 실행 시간(TIME+), 명령어(CMD) 등이 표시

top 명령어의 상호작용 키
h: 도움말 표시
q: top 명령어를 종료
k: 프로세스 종료, PID 입력
r: 프로세스 우선순위 변경
u: 특정 사용자의 프로세스만 표시
p: CPU 사용률을 기준으로 정렬
M: 메모리 사용률을 기준으로 정렬
N:PID를 기준으로 정렬
T: 실행시간을 기준으로 정렬
c: 전체 명령어 라인을 표시하거나 숨김
1: 각 CPU 코어별 사용량을 표시

-b: 배치 모드롤 실행
-n: 출력할 갱신 횟수를 지정
-u: 특정 사용자의 프로세만 표시

<img width="854" alt="image" src="https://github.com/ssswoowoook/opensw/assets/170293211/0afc969c-bfa8-477e-b33a-752412502fbd">

top 명령어는 리눅스 시스템 관리자가 시스템 성능을 모니터링하고 문제를 해결하는 데 필수적인 도구이다. 시스템 자원을 효율적으로 관리하고, 문제 발생 시 빠르게 대응 가능

##ps
