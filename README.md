# GitFlowZero
깃 테스트.
- git reset 명령어는 잘 못하니 GUI 를 이용해서 작업하는데, 헷갈리는 부분이 있다.
- 아래의 내용들은 `local branch` 에서 구동하는 것이 아니라 `remote branch` 에서 같이 이력이 관리되고 있는 상태이다.
- `local brach` 에서만 이력이 관리되고 있다면 `git reset hard` 는 __매우 신중하게 하여야 한다.__

## 이 커밋까지 현재 브랜치를 초기화.
`이 커밋까지 현재 브랜치를 초기화. `
![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(1).png)

## git reset soft
- 돌아가려 했던 이력으로 되돌아간다.
- 모든 로컬 변경사항을 유지.
- 로컬 상에 있는 브랜치만 리셋된다.
  - 다시 커밋할 수 있는 상태가 되고 `git pull origin master` 또는 소스트리 내의 `pull` 버튼을 통해서 다시 리모트 브랜치의 이력을 추적할 수 있다.
  
![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20soft.PNG)
![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20soft%20%EC%9D%B4%ED%9B%84%20%EA%B2%B0%EA%B3%BC..PNG)

## git reset mixed
- 돌아가려 했던 이력으로 되돌아간다.
- 작업했던 작업물들은 `unstaged area` 에 올려져 있고, 해당 내용들은 `commit & push & pull` 을 통해서 다시 합칠 수 있다.

![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20mix.PNG)
![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20mix%20%EC%9D%B4%ED%9B%84%20%EA%B2%B0%EA%B3%BC..PNG)
![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20mix%20%EC%9D%B4%ED%9B%84%20%EA%B2%B0%EA%B3%BC.%20(2).PNG)

## git reset hard
- 돌아가려 했던 이력으로 되돌아간다.
- `local branch` 가 작업했던 작업물들은 전체가 사라졌다.
- `git pull` 명령어를 통해서 `remote branch` 와 동기화를 수행하거나 그 외적인 부분은 전적으로 이력관리를 수행하는 사람에게 달려있다.

![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20hard.PNG)
![](https://github.com/pasudo123/GitFlowZero/blob/master/images/%EC%86%8C%EC%8A%A4%ED%8A%B8%EB%A6%AC%20(2)%2C%20hard%20%EC%9D%B4%ED%9B%84%20%EA%B2%B0%EA%B3%BC.PNG)
