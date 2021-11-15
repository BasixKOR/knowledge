---
title: WSL
---

- [[Windows]] Subsystem for [[Linux]]. Windows에서 Linux 환경을 사용하기 위해 제공되는 확장 기능이다.

- 현재 [[Windows]]에서 권장되는 [[POSIX]] 호환 환경이다.

- 1과 2의 차이
	 - https://docs.microsoft.com/en-us/windows/wsl/compare-versions

	 - https://thecodeblogger.com/2020/08/22/understanding-differences-between-wsl-1-and-wsl-2/

	 - WSL 1
		 - 기본적으로 Linux의 syscall을 즉석에서 상응하는 Windows WinAPI 호출로 변환하는 방식으로 동작했다.

		 - 이러한 구조는 [[VM]]의 overhead 없이 Linux를 사용 가능하게 해 주었지만 사용 가능한 syscall에 제한이 따랐고 그로 인해 사용할 수 있는 소프트웨어에도 제한이 있었다.

	 - WSL 2
		 - Hyper-V 가상화 기술을 이용해서 일종의 경량화된 Linux [[VM]]을 제공한다.

		 - [[Microsoft]]에서 WSL을 위해 최적화한 [[Linux]] 커널이 제공된다.

		 - RAM을 많이 먹고 Windows-WSL 간 파일 전송이 끔찍하게 느린 점을 제외하면 전반적으로 개선되는 점이 많다.
