---
title: CLI
---

- 커맨드-라인 인터페이스.

- 어떻게 만들어야 하는가
	 - [POSIX.1-2017 12.2 Utility Syntax Guidelines](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap12.html)
		 - [[POSIX]] 표준에서 권장되는 CLI 프로그램의 옵션 및 인자 전달 방식.

		 - 대시(-)를 이용한 옵션 전달 방식의 시초가 된다.

	 - [The GNU C Library Reference Manual, 25.1.1 Program Argument Syntax Conventions](https://www.gnu.org/software/libc/manual/html_node/Argument-Syntax.html)
		 - `--something` 과 같은 긴 형태의 옵션은 여기서 [[GNU]] 확장으로 처음 등장했다.

		 - `--name=value` 형태로 인자를 제공하는 것이 GNU의 권장 사항이지만 요즘은 그냥 `--name value` 해도 되는 것 같다.

	 - [Command Line Interface Guidelines](https://clig.dev/)
		 - 위의 두 가이드는 나보다 나이를 먹었기 때문에 현대 컴퓨팅 환경에 맞춰서 작성된 가이드라인이다.

		 - Git 등의 CLI 소프트웨어에서 흔히 보이는 서브커맨드 등을 고려 대상으로 삼고 있다.

		 - 상황에 따라 interactive하지만 machine-readable한 데이터 역시 받아올 수 있도록 디자인하는 방식을 제안한다.

		 - `--json`, `--help`, `--no-input`, `--plain`, `--no-color` 등 구현하여야 하는 옵션의 이름을 명확하게 제안한다.

		 - [12 Factor CLI Apps](https://medium.com/@jdxcode/12-factor-cli-apps-dd3c227a0e46)
			 - [[The twelve-factor app]]에서 영감을 얻은 네이밍인듯
