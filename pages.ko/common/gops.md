# gops

> 현재 시스템에서 실행중인 Go 프로세스를 나열하고 진단.
> 더 많은 정보: <https://github.com/google/gops>.

- 로컬에서 실행되는 모든 go 프로세스를 출력:

`gops`

- 프로세스에 대한 추가 정보를 출력:

`gops {{프로세스아이디}}`

- 프로세스 트리 출력:

`gops tree`

- 대상 프로그램에서 현재 스택 추적 현황을 출력:

`gops stack {{프로세스아이디|주소}}`

- 현재 런타임 메모리 통계를 출력:

`gops memstats {{프로세스아이디|주소}}`
