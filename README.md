# VR-Avalon
VR avalon for Oculus

## 개요
### 오큘러스로 플레이 하는 avalon

5인에서 최대 10인까지 플레이 가능한 멀티 게임.

악당이 여럿이 존재하며 그들을 피해서 총 3라운드를 이겨야 선의 승리.
반대로 총 3라운드를 방해하면 악의 승리.
악과 선의 싸움으로 5판 3선승제 이다.
이때, 악은 3라운드를 져도 마지막에 선의 리더를 고르면 역전승이 가능하다.

Unity3D

platform : Oculus
Server : photon fusion (무료 버전)

---

## 목표
### 3D 환경에서 아바타를 이용한 상호작용이 가능한 아발론 게임 진행

1. Lobby : 최소 5인 에서 최대 10인이 입장가능한 방 제작
 - 랜덤 입장(닉네임 필수)
 - 레디 기능
 - 방장은 게임에서 가능한 캐릭터 / 기능(엑스칼리버, 호수의 여신) 등을 On/Off 가능 (추후 추가)
 - 모두 레디시 방장이 플레이버튼으로 진입
 - 이때, 인원에 따라 각 판수의 모험인원을 자동으로 지정받는다.
 
2. Avatar : 각 유저들의 고유한 능력들을 보유함. 
 - 머리위에 필요한 경우 머리위에 닉네임이 보임. (본인이 악을 아는 경우 : 닉네임이 빨간색)
 - 손바닥으로 본인의 직업을 확인할 수 있음.
 - 고정된 위치에서 머리와 손을 움직일 수 있음.
 - 물건을 집거나 버튼을 누를 수 있음.
 
3. Table : 게임을 순서대로 진행하게 함.
 - 방장부터 원정대장이 되어 모험을 갈 사람들을 클릭하고, 모두 고르면 버튼이 활성화 되어 버튼을 누르면 모험을 보낸다. (선택된 사람 재 클릭시 선택 해제)
 - 다른 플레이어 들은 선택이 종료되면 해당 모험을 찬/반 할 버튼이 생긴다. (찬/반 버튼은 좌우 랜덤)
 - 해당 찬/반이 과반수 이상이면 선택된 사람들은 성공 실패를 고른다. (성공/실패 버튼은 좌우 랜덤)
 - 해당 방식으로 총 5라운드를 진행해서 결과를 도출한다.
 - 이때, 악이 승리하면 암살자는 멀린을 클릭해서 고르고, 고르면 버튼이 활성화 되어 버튼을 누르면 멀린인지 판단한다.

## 규칙
### 게임 진행 방식 설명

1. 방장이 로비에서 게임 시작하면 방에 입장한다.
2. 각 유저들은 원형 테이블에 앉아 게임을 시작한다.
3. 각 유저들은 머리위에 닉네임이 보이고, 만약, 악이거나 멀린이면 악인 닉네임은 빨간색으로 보인다.
4. 각 유저들은 손바닥으로 자신의 직업과 승리조건을 알 수 있다.
5. 방장부터 원정대장이 된다.
6. 원정대장은 모험을 갈 사람을 지목 / 클릭으로 모험갈 사람을 지정한다.
7. 이미 선택된 사람을 지정하면 선택이 해제된다.
8. 모험갈 사람을 모두 지정하면 원정대장 앞에 버튼이 활성화 된다.
9. 앞으로 나올 모든 버튼들은 해당하는 사람에게만 보인다.
10. 원정대장이 버튼을 누르면 다른 유저들은 앞에 버튼이 활성화 된다(찬/반)
11. 찬반 버튼은 좌우 랜덤하게 나오고, 본인에게만 보인다.
12. 버튼을 눌러서 과반수가 나오면 모험을 떠남.
## 구조
