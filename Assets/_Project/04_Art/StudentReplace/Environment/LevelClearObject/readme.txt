스테이지 클리어 오브젝트 리소스 넣는 곳
(UI 화면이 아니라, 스테이지 안에 실제로 놓여서 플레이어가 공격해서 맞히면 스테이지 클리어가 되는 오브젝트입니다 - 닿기만 해서는 안 됩니다. 예: 깃발, 문, 보물상자 등 원하는 그림으로)

파일:
  level_clear_object.png   500x500px 정사각형 - 캔버스 크기는 그대로, 안의 그림 모양은 자유

규칙:
  - PNG, 알파 채널 투명
  - ★ 물건의 밑동을 캔버스 맨 아래에 붙여 그릴 것 - 캔버스 아래 선이 곧 땅입니다
    (씬에 놓인 높이 Position Y -0.9 가 "캔버스 아래 선 = 바닥"인 자리라서,
     캔버스 한가운데에 그리면 공중에 뜹니다. Unity 기준점 자체는 가운데(Center)입니다)
  - 캔버스 크기는 500 x 500 그대로 - 바꾸면 땅에 묻히거나 떠서 Position Y 를 다시 맞춰야 합니다
  - 캐릭터와 비슷한 크기감으로 작업하면 자연스럽습니다 (너무 작거나 크면 배치 후 눈으로 보고 조정)

넣는 법 (5주차 - 배경과 함께):
  BackgroundTest 씬에는 LevelClearObject 가 이미 놓여 있습니다.
  level_clear_object.png 를 같은 이름으로 덮어쓰기만 하면 그림이 바뀝니다 (도구 필요 없음).
  위치는 Hierarchy 에서 LevelClearObject 를 선택해 Position X 로 스테이지 끝에 옮기세요.
  ★ 닿는 게 아니라 "공격해서 맞혀야" 클리어됩니다 (테스트는 Ctrl+L).

  씬에 LevelClearObject 가 아예 없을 때만 `Add Stage Start & Clear To Background Test Scene` 도구로
  추가합니다 (이미 있으면 그 도구는 위치를 건드리지 않습니다).

자세한 내용:
  https://github.com/hansung-game1/game-p-docs/blob/main/주차별수업/W05_배경_스테이지1%28기본%29.md
