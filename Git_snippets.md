Git:
-----------

		Github HELP:
		------------
			setup an action: https://help.github.com/en/actions

  git config --list

  // sets the new remote
  git remote add origin remote <repository_URL>
  // verifies remote
  git remote -v

  // Pushes the changes in your local repository up to the remote repository you specified as the origin
  git push origin master

  // git config --global http.proxy http://127.0.0.1:8888
  The setting can be disabled through the following Git command:
	git config --global --unset http.proxy

    Stashing:
	---------
		git stash save “Your stash message”.
			-u is for untraced files
		git stash list
		git stash apply stash@{1}
		clear all the stashes in the repo:   Git stash clear
   git push -u origin feature/GIN-505_urls


   git push --set-upstream origin feature/GIN-25_TextePremiumScreen


   git reflog
   
   git reset --hard HEAD
   
   // throuw all commits and reset to dovelop
	git fetch origin
	git reset --hard origin/develop
   
   // remove all changes and commits
	git reset --hard HEAD
	// 3333333git pull --strategy=theirs git@github.axa.com:esales/es-ui.git
	git fetch origin
	git reset --hard origin
	
	throwing local commits:
		git reset --hard origin/master

   
   merging:
   --------
   in master:
		git merge --squash feature
		git commit -m "merget from feature"

   or in feature:
		git rebase master
			// we rebase the feature branch to start from the HEAD of master
		
   origin and remote repository aliaces:
   -------------------------------------
   $ git remote -v
	origin  git@github.axa.com:esales/es-ui.git (fetch)
	origin  git@github.axa.com:esales/es-ui.git (push)



 SSH key:
 --------

	Adding git SSH key to the git agent and then to the github:
		 ssh-keygen -t rsa -b 4096 -C "elitsa.mladenova@axa-winterthur.ch"
		 eval `ssh-agent -s`
		 ssh-add ~/.ssh/id_rsa
 
 
 Git cert	KeyPass:
 --------
	privat
	/git-repos/esales-infrastructure:	
		7fF925B83b8367c876W430c63Aa80032
	AXA Git Bash :	68382af3f8d3a2db53f9b6e0ab56fe32ab835c8b
		// This has to be given in the windows credential manager as password for my github username
		
		monitoring:
			E906464
			dhhRocks2019

			

   $ git config -l
		http.sslcainfo=C:/eplatform/tools/Git/mingw64/ssl/certs/ca-bundle.crt
		http.sslbackend=openssl
		diff.astextplain.textconv=astextplain
		filter.lfs.clean=git-lfs clean -- %f
		filter.lfs.smudge=git-lfs smudge -- %f
		filter.lfs.process=git-lfs filter-process
		filter.lfs.required=true
		credential.helper=manager
		http.sslverify=false
		http.proxyauthmethod=basic
		http.proxy=http://127.0.0.1:8888
		user.name=elitsaml
		user.email=elitsa.mladenova@gmail.com
		https.sslverify=false
		core.repositoryformatversion=0
		core.filemode=false
		core.bare=false
		core.logallrefupdates=true
		core.symlinks=false
		core.ignorecase=true
		remote.origin.url=https://github.com/axa-ch/pod-rsv.git
		remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
		branch.master.remote=origin
		branch.master.merge=refs/heads/master
		branch.develop.remote=origin
		branch.develop.merge=refs/heads/develop
		branch.feature/GIN-1809_Number_of_Adults.remote=origin
		branch.feature/GIN-1809_Number_of_Adults.merge=refs/heads/feature/GIN-1809_Number_of_Adults
		user.email=elitsa.mladenova@gmail.com

		Urs config:
		-----------
		$ git config -l
		http.sslcainfo=C:/eplatform/tools/Git/mingw64/ssl/certs/ca-bundle.crt
		http.sslbackend=openssl
		diff.astextplain.textconv=astextplain
		filter.lfs.clean=git-lfs clean -- %f
		filter.lfs.smudge=git-lfs smudge -- %f
		filter.lfs.process=git-lfs filter-process
		filter.lfs.required=true
		credential.helper=manager
		user.name=urs-wiss
		user.email=urs.wiss@axa-winterthur.ch
		core.autocrlf=true
		http.proxy=http://localhost:8888
		https.proxy=http://localhost:8888
		core.repositoryformatversion=0
		core.filemode=false
		core.bare=false
		core.logallrefupdates=true
		core.symlinks=false
		core.ignorecase=true
		remote.origin.url=https://github.com/axa-ch/pod-rsv.git
		remote.origin.fetch=+refs/heads/:refs/remotes/origin/
		branch.master.remote=origin
		branch.master.merge=refs/heads/master
					

		Fiddler:
		   settings: connection  Bypass:
			<-loopback>;npmjs.org;github.com;bower.herokuapp.com;github.axa.com

