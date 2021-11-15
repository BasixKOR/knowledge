---
title: Git
---

- Linus Torvalds가 다른 형상 관리 도구 쓰다가 맘에 드는 게 하나도 없다고 직접 만들어 쓰기 시작해서 이제 다들 쓰는 형상 관리 도구.

- 팁
	 - Shallow clones
		 - 아주 커다란 Git 저장소를 가져올 때 과거 커밋에 접근할 필요가 없다면 fetch나 clone 시 `--depth 1` 옵션을 이용해 shallow clone을 만들 수 있다.
			 - 이후 과거 커밋이 필요하다면 `git fetch --unshallow` 를 하면 된다.

	 - Submodules
		 - `git submodule update --init --recursive` 를 하면 HEAD의 상태로 서브모듈들을 잘 동기화해준다.

	 - [Git For Windows는 기본적으로 Symbolic Link 기능이 꺼져 있다](https://github.com/git-for-windows/git/wiki/Symbolic-Links)
#Windows
		 - 켜려면 `git config core.symlinks true` 등으로 임의로 켜 줘야 함

	 - Fast-forward 머지는 checkout하지 않아도 할 수 있다
		 - `git fetch origin main:main` 하면 main 브랜치가 Fast-forward 된다

	 - fetch할 때 업데이트되는 브랜치는 refspec에 따라 정해진다
		 - [[GitHub]] CLI는 포크된 저장소를 클론할 때 upstream의 refspec을 주요 브랜치 하나로 한정하므로 기억해두는 편이 좋다

		 - [간단한 설명](https://stackoverflow.com/a/39957858)

	 - 변경 사항을 Pull Request나 브랜치 등을 거치지 않고 빠르게 공유할 필요성이 있는 경우 Git의 [format-patch](https://git-scm.com/docs/git-format-patch)와 [am](https://git-scm.com/docs/git-am) 커맨드를 활용할 수 있다.
		 - https://www.git-tower.com/learn/git/faq/create-and-apply-patch/

		 - 실제로 [[Linux]]와 같은 오래된 프로젝트는 메일링 리스트에 이러한 patch 파일을 보내 Pull Request와 유사하게 사용한다.

		 - 잘 알려지지 않은 기능이다 보니 사용할 때 동료들에게 사용 방법도 귀띔해주길 권한다.

	 - [git bundle](https://git-scm.com/docs/git-bundle)을 통해 지금까지 작업한 브랜치(편의상 이렇게 부르자)를 한 파일로 합쳐 공유할 수 있다.

	 - gitignore 소스는 여기 있는 거 배껴쓰면 편하다
		 - https://www.toptal.com/developers/gitignore

		 - Yarn의 경우는 ((a53edc88-9978-4df6-941a-52498dd67300)) 참조
