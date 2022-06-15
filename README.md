# C++SnakeGame

key 변수 선언위치 변경

gate1X, gate1Y, gate2X, gate2Y 변수 추가(2개의 게이트의 좌표변수)

setKey 추가

랜덤난수 출력 메서드 추가

board 규칙 추가 - -2 : Gate 없는 벽 (벽으로 둘러싸여 있어 접촉할 수 없기에 기능 추가 x)

랜덤 난수를 이용한 게이트 생성 코드 추가 (initSnakeBoard)

ImmuneWall 설정 메서드 추가(추가 스테이지를 감안하여 구현한 메서드이기에 아직 시행해보지 않음)

gate 출입 시 이동 메커니즘 추가 (moveSnake : 매개변수 int enterGate 추가)

enterGate 메서드 추가 (Gate 출입 시 상황에 맞는 키 리턴, 외각 Gate일 경우 나오는 방향 고정, 내부에서 생성된 게이트일 경우 정방향, 우측, 좌측, 반대방향 순으로 진행)

snakeLength가 2 이하일 경우 패배하도록 수정


2022.06.15. 17:45

게이트 생성 코드 삭제(initSnakeBoard) 및 게이슽 생성 메서드 추가 (setGate)
추가 스테이지 및 추가 코드에 맞춰 내용 수정


2022.06.15. 23:05

점수판 UI 추가

2022.06.15. 23:42

아이템 랜덤 생성 및 미션 수정

2022.06.16. 01:00

addItem 메서드 삭제 및 locateItem 메서드 추가

locate 메서드는 기존의 존재하던 아이템을 삭제한 후 아이템을 배치하는 기능 수행

moveSnake 메서드 내 locateItem 메서드를 추가하여 아이템 습득 후 아이템 재배치 수행

아이템 재배치가 일정 시간 마다 수행하도록 로직 변경(Growth와 Poison의 재배치 시간 차별화)
