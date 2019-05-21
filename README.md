# logging.101.camp
> auto deploy logging br.

## init.

    ༄  mkdir dlog_gh_101camp

    ༄  cd dlog_gh_101camp/

    ༄  git init .
    Initialized empty Git repository in /opt/data/Sites/101.camp/_running/dlog_gh_101camp/.git/

    ༄  git remote add -t dlog101camp -f origin  git@github.com:101camp/comments.git
    Updating origin
    remote: Enumerating objects: 4, done.
    remote: Counting objects: 100% (4/4), done.
    remote: Compressing objects: 100% (3/3), done.
    remote: Total 4 (delta 0), reused 4 (delta 0), pack-reused 0
    Unpacking objects: 100% (4/4), done.
    From github.com:101camp/comments
     * [new branch]      dlog101camp -> origin/dlog101camp

    ༄  git co dlog101camp
    Branch dlog101camp set up to track remote branch dlog101camp from origin.
    Switched to a new branch 'dlog101camp'

    ༄  git br -a
    * dlog101camp
      remotes/origin/dlog101camp

