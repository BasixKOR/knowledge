---
title: Scoop
---

- https://scoop.sh/

- 소개
	 - [[Windows]]를 위한 [[패키지 매니저]].

	 - 사용자 디렉토리에 패키지를 설치하고 관리해주는 소프트웨어.

	 - PowerShell 기반으로 작성되어 있음

	 - bucket이라는 저장소 안에 여러 패키지 정보가 저장되어 있고, 이러한 bucket에서 받은 패키지 명세를 바탕으로 패키지를 설치 및 관리하는 구조
		 - [Scoop Directory](https://rasa.github.io/scoop-directory/)에 이러한 Bucket들의 목록이 있다.

	 - GUI 프로그램은 설치하면 자주 시작 메뉴 엔트리가 사라지거나 해서 [[CLI]] 프로그램 관리에만 쓰는 게 sweet spot인 듯

- Buckets
	 - https://github.com/ScoopInstaller/Main
		 - 처음 깔면 딸려온다.

		 - 등재를 위한 [나름 깐깐한 규정](https://github.com/ScoopInstaller/Scoop/wiki/Criteria-for-including-apps-in-the-main-bucket)이 있다.

	 - https://github.com/ScoopInstaller/Extras
		 - Main bucket의 기준에는 안 맞지만 쓸모 있는 것들

	 - https://github.com/chawyehsu/dorado
		 - 왠지 main이나 extras에 있어야 할 것 같은데 없는 잡다한 것들이 들어가 있다.

		 - 이미 main이나 extras에서 제공되는 것들의 변형판을 받기 좋은 듯

	 - https://github.com/TheRandomLabs/scoop-nonportable
		 - 포터블하지 않은 앱들을 담아두는 곳

	 - https://github.com/ScoopInstaller/Java
		 - [[Java]]의 여러 배포판들을 모아두고 있다.

		 - 여담이지만 Scoop로 Java 설치를 관리하는 건 별로 좋은 생각이 아니다.

- [Shovel](https://github.com/Ash258/Scoop-Core)
	 - Ash258이 Scoop이 일부 기능 업데이트 느린 게 마음에 안 들었는지 만든 Scoop의 변형판이다.

	 - 일부 특이한 변경 사항을 제외하면 다시 Scoop로 기여하기도 하는 등 업스트림과의 사이는 좋아 보이는 편

	 - Shovel에서만 지원되는 기능들
		 - Zstd 압축 해제 지원

		 - VirusTotal 검사 지원

		 - arm64 지원

		 - JSON 외 포맷으로 작성된 패키지 명세 지원

		 - GitHub rate limiting 방지

		 - Scoop bucket 관리자를 위한 편의 기능
