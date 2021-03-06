# github flow

1. master 브런치는 어떤 때든 배포가 가능하다.
master 브런치는 항상 최신의 상태이며, stable 상태로 Product에 배포되는 브런치이다. 그리고 이 브런치에 대해서는 엄격한 role를 주어 사용한다.

2. 새로운 일을 시작하기 위해 브런치를 master에서 딴다면 이름은 어떤 일을 하는지 명확하게 작성한다.
git flow 와는 다르게 feature 브런치나 develop 브런치가 존재하지 않는다. 그렇기에 새로운 기능을 추가하거나 버그를 해결하기 위한 브런치의 이름은 자세하게 어떤 일을 하고 있는지에 대해서 작성해주도록 하자. Github 페이지에서 보면 어떤 일들이 진행되고 있는지를 확인하기 쉽게 말이다.

3. 원격지 브런치로 수시로 push를 한다.
git flow 와 가장 상반되는 방식이다. 항상 원격지에 자신이 하고 있는 일들을 올려 다른 사람들도 확인할 수 있도록 해준다.
이 방법의 좋은 점은 하드웨어에 문제가 발생하여 작업하던 부분이 없어지더라도 원격지에 있는 소스를 받아서 작업을 할 수 있도록 해준다.

4. 피드백이나 도움이 필요할 때, 그리고 머징 준비가 완료되었을 때는 pull request를 생성한다.
pull request 는 코드 리뷰를 도와주는 시스템이다.
그렇기에 이것을 이용하여 자신의 코드를 공유하고, 리뷰를 받을 수 있도록 한다. 물론 머지가 준비 완료되어 master 브런치로 반영을 요구하여도 된다.

5. 기능에 대한 리뷰와 사인이 끝난 후 master로 머지한다.
곧장 product로 반영이될 기능이기에 이해관계가 연결된 사람들과 충분한 논의 이후 반영하도록 한다.

6. master로 머지되고 푸시되었을 때는 즉시 배포되어야 한다.
GitHub Flow의 핵심인듯한 master로 머지가 일어나면 hubot을 이용하여 자동으로 배포가 되도록 설정해놓는다.