# git

## git 기본설정 : Basic Config for git 

    git config --global user.name "[Your Name]"
    git config --global user.email [Your Email]
    git config --global color.ui true
    git config --global core.autocrlf input
    git config --global push.default simple
    git config --global pull.rebase true
    git config --global rerere.enabled true
    git config --global alias.s "status -s"
    git config --global alias.lg "log --oneline --decorate --all --graph"
    printf '.idea/\n.DS_Store\n' > .gitignore_global
    git config --global core.excludesfile ~/.gitignore_global

    

* References
  * [Git 최초설정 (git-scm)](https://git-scm.com/book/ko/v2/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EC%B5%9C%EC%B4%88-%EC%84%A4%EC%A0%95)
  * [Git 맞춤설정 (git-scm)](https://git-scm.com/book/ko/v2/Git%EB%A7%9E%EC%B6%A4-Git-%EC%84%A4%EC%A0%95%ED%95%98%EA%B8%B0)
  * [Mastering GitHub (Code School)](http://campus.codeschool.com/courses/mastering-github/level/1/section/1/video/1)
 
## git 설치 : Install git

### For Ubuntu
- sudo apt-get update
- sudo apt-get install git