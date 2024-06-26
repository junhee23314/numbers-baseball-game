# [숫자 야구 게임⚾]

*** 게임설명: *** 
컴퓨터가 랜덤으로 생성한 세 개의 숫자를 사용자가 맞추는 것입니다. 각 숫자는 1부터 9까지의 범위에 있으며, 중복되지 않습니다. 
스트라이크와 볼의 수를 통해 피드백을 받습니다. 사용자는 숫자와 위치를 맞추는 게임입니다.

![숫자야구게임_1](https://github.com/junhee23314/numbers-baseball-game/blob/main/%EC%88%AB%EC%9E%90%EC%95%BC%EA%B5%AC%EA%B2%8C%EC%9E%84%EC%9D%B4%EB%AF%B8%EC%A7%80_1.png)

# 1. 컴퓨터가 0~9까지 3개의 서로 다른 난수를 발생시킨다.  
 난수발생 메소드 - 난수를 9로 나눈 나머지+1
 서로 다른 수 => do while을 사용하여 난수를 먼저 발생시키고 서로 다른 수가 될 때까지 반복
 서로 다른 난수 세 개 반환

# 2. 사용자는 0~9까지의 3개의 서로 다른 숫자를 입력한다.
  게임 플레이 메소드 - 게임 시도 횟수, 사용자가 입력하는 3개의 숫자 배열, 컴퓨터가 발생시킨 난수 배열, strike과 ball 개수 파악
 컴퓨터가 발생시킨 난수와 사용자가 입력한 숫자를 비교한다.
 자리의 크기까지 같으면 strike을 증가: 배열을 이용하여 완벽히 일치하는지
  숫자의 크기만 같으면 ball을 증가: 배열의 자리가 다른 숫자끼리 각각 비교
 게임은 정해진 시도횟수까지 반복, 또는 3 strike 일 때  종료
 게임 시도횟수를 반환

# 3. 메인메소드: 시도횟수에 따라 출력메시지를 다르게 출력
