---
title: MSYS2
---

- 소개
	 - Cygwin과 MinGW-w64의 커스텀 빌드를 조합하여 [[POSIX]] 환경과 유사한 빌드 환경을 제공해주는 소프트웨어 패키지

	 - 본인은 마음대로 쉘 대용으로 쓰고 있음

	 - [[Arch Linux]]의 [[패키지 매니저]]인 pacman을 사용하여 패키지를 관리
		 - 패키지 목록은 [여기](https://packages.msys2.org/)에서 볼 수 있다

- 여러가지 설정 방법
	 - [Install inside MSYS2 proper - Git for Windows](https://github.com/git-for-windows/git/wiki/Install-inside-MSYS2-proper)
id:: 7f2eb350-2c5e-4340-ace0-99ded3eab9ea
		 - 공식적으로 지원되는 방법은 아니나 Git For Windows (MSYS2 기반)의 패키지를 끌어다 쓰면 됨

	 - [How to change HOME directory and start directory on MSYS2?](https://stackoverflow.com/questions/33942924/how-to-change-home-directory-and-start-directory-on-msys2)
		 - 위의 ((7f2eb350-2c5e-4340-ace0-99ded3eab9ea))를 했다면 이미 적용되지만, [[Scoop]] 등으로 [[Git]]을 별도로 설치하고자 하는 경우 필요함

	 - [MSYS2-Introduction # PATH](https://www.msys2.org/wiki/MSYS2-introduction/#path)
		 - [[Windows]]에서 별도로 설치한 [[CLI]] 도구를 사용하기 위해 필수적이다.

		 - msys2-shell.cmd 에 별도 인자를 주어 설정할 수도 있다.
