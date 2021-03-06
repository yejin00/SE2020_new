# SE2020_new

# Workflow Scenario

## 1. Git branch
  <pre><code>
master : 제품으로 출시될 수 있는 브랜치
develop : 다음 출시 버전을 개발하는 브랜치
feature : 기능을 개발하는 브랜치
release : 이번 출시 버전을 준비하는 브랜치
hotfix : 출시 버전에서 발생한 버그를 수정 하는 브랜치
  </code></pre>

## 2. Git Workflow
  <pre><code>
  1. 깃허브 repository에서 나의 repository에 fork한다.
  
  2. 나의 repository에서 local로 가져오기 위해 clone한다.
  
  3. 내가 fork한 주소를 local로 가져오고, 이를 상대방 repository와 연결한다.
  &nbsp;&nbsp;&nbsp;&nbsp; $ git remote add pair Repo URL for pairs fork
  
  4. 코드를 작성한 후 add, commit을 실행한다.
  &nbsp;&nbsp;&nbsp;&nbsp; $ git add change file
   &nbsp;&nbsp;&nbsp;&nbsp;$ git commit -m "commit message"
   
  5. 나의 repository에 push 한다. 
   &nbsp;&nbsp;&nbsp;&nbsp;$ git push origin master
   
  6. 내가 commit하고 push하여 변경된 내용을 상대방은 git pull을 통해 
     자신의 local repository로 가져올 수 있다. 
  &nbsp;&nbsp;&nbsp;&nbsp; $ git pull pair master (or other branch name)

  7. 주의사항은 local로 clone 했을 시, local로만 개발할 수 없기 때문에 master repository와 
     연결을 해주어야 한다. master repository에 업데이트 되는 새로운 내용, 변경 사항들을 
     수시로 pull을 해서 local을 맞춰줘야 한다. 
  </code></pre>

  ![workflow](https://user-images.githubusercontent.com/55871397/95009116-679b8200-065a-11eb-8f86-f0309eaf6ddb.jpg)


