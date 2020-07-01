# Git 시작하기

## add

커밋할 대상을 목록에 추가하는 명령어입니다.

## commit

변경된 정보를 확정해서 기록하는 명령어입니다.

## clone

Git 디렉토리는 Git이 프로젝트의 메타데이터와 객체 데이터베이스를 저장하는 곳을 말한다. 
이 Git 디렉토리가 Git의 핵심이다.
다른 컴퓨터에 있는 저장소를 Clone 할 때, Git 디렉토리가 만들어진다.

다른 프로젝트에 참여하거나 Git 저장소를 복사하고 싶을 때, `git clone`명령을 사용한다.
`git clone` 을 실행하면 프로젝트 히스토리를 전부 받아온다.

`git clone [url]` 명령으로 저장소를 clone 한다.

```bash
$ git clone https://github.com/xxxx/yyyy
```

## pull

리모트 저장소를 관리할 줄 알아야 다른 사람과 함께 일할 수 있다. 리모트 저장소는 인터넷이나 네트워크 어딘가에 있는 저장소를 말한다. 저장소는 여러 개가 있을 수 있는데 어떤 저장소는 읽고 쓰기 모두 할 수 있고 어떤 저장소는 읽기만 가능할 수 있다. 간단히 말해서 다른 사람들과 함께 일한다는 것은 리모트 저장소를 관리하면서 데이터를 거기에 Push 하고 Pull 하는 것이다.

remote respository에서 데이터를 가져오려면 아래와 같은 명령어를 입력한다.

```bash
$ git pull
```

그냥 쉽게 git pull 명령으로 리모트 저장소 브랜치에서 데이터를 가져올 뿐만 아니라 자동으로 로컬 브랜치와 Merge 시킬 수 있다.

## push

프로젝트를 공유하고 싶을 때 Upstream 저장소에 Push 할 수 있다. 이 명령은 git push [리모트 저장소 이름] [브랜치 이름]`으로 단순하다.(((git commands, push))) master 브랜치를 `origin서버에Push 하려면(다시 말하지만 Clone 하면 보통 자동으로 origin 이름이 생성된다) 아래와 같이 서버에 Push 한다.

```bash
$ git push origin master
```
