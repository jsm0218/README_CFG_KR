# Configurable SD/USB Loader v70r78 MOD patched

![enter image description here](https://cdn.discordapp.com/attachments/1061501682741157890/1285385095112298547/intro4.jpg?ex=66ea13a7&is=66e8c227&hm=ffd97797f718892f94bf31d9b0476ef02ad4214bf233655b18541239599ad9ec&)

oggzee, usptactical, gannon & Dr. Clipper에 의해 제작

이 버전의 로더는 다양한 옵션을 사용자 정의하여 사용자의 기본 설정에 더 잘 맞출 수있게합니다.

Wanikoko SD/USB Loader 1.5, Kwiirk Yal&cios 222, Hermes uLoader 1.6&cios 222/223 + mload + 많은 다른 것들을 기반으로합니다.
(Sorg, nIxx, fishears, usptactical, 56Killer, WiiShizzza, hungyip84, Narolez, ...)


## 기능

 - SDHC, USB HDD 장치 지원
 - GUI (그리드 / 커버플로우) 와 컨솔 모드 (런타임 시 전환 가능)
 - 배경 음악 (.mp3 또는 .mod)
 - 테마 (런타임 시 전환 가능)
 - 테마 브라우져
 - 와이드스크린 (자동-검색)
 - 투명도 (커버와 컨솔)
 - 커버 이미지 다운로드
 - 커버 스타일: 2D, 3D, 디스크, 모두
 - 커버 자동 크기 조정
 - 게임 타이틀의 이름 변경 (titles.txt, custom-titles.txt 및 / 또는 wiitdb.zip 사용)
 - 비디오 모드, 언어, 오카리나 치팅의 게임 별 구성
 - 설치가 완료되면 DVD 슬롯에 불이 들어오고, 추가적으로 꺼내기
 - 자녀 보호
 - 여러 파티션이 지원되는 USB HDD
   (게임용 WBFS 및 설정, 표지 및 기타 리소스 용 FAT)
 - 여러 파티션이 지원되는 SDHC
   (게임용 WBFS 및 리소스 용 FAT...)
 - USB 드라이브 및 기타 USB 장치와의 호환성을 향상시키기위한 사용자 지정 IOS 선택.
 - cIOS 지원:
   davebaol d2x (추천)
   waninkoko 247, 248, 249 & 250
   Hermes 222, 223 & 224 (mload)
   kwiirk 222 & 223 (yal)
 - 배너 사운드
 - Wii의 플레이 로그에 게임 플레이 시간 저장
 - 여러 WBFS 파티션 지원
 - FAT 또는 NTFS 파티션에서 게임 불러오기
   (cIOS 222/223 rev4 이상 또는 cIOS 249 rev18 이상 요구)
 - 지원되는 게임 디스크 파일 형식 : .wbfs 와 .iso
 - 구성 가능
 

최신 뉴스, 질문 및 제안은 여기를 클릭합니다:
http://gbatemp.net/index.php?showtopic=147638


## 설치

"inSDroot"의 내용을 SD 카드의 루트에 복사합니다.
그러면 USB 로더가 자작 채널에 추가됩니다.
채널 포워더를 설치하여 시스템 메뉴에서 직접 로더를 시작할 수 있습니다.
(참고 : 대체로, USB FAT 파티션을 사용하여 구성 및 커버를 저장할 수 있습니다.)

## 유용한 링크

Wii 홈브류 및 Cfg의 단계별 설치 지침:
http://gwht.wikidot.com

포워더는 여기에서 다운로드 할 수 있습니다.:
http://gbatemp.net/index.php?showtopic=147638&st=5745&p=2420653&#entry2420653
그리고 WAD 매니저와 함께 설치됩니다.

게임 커버 이미지들은 여기에서 다운로드 할 수 있음:
http://wiitdb.com

업데이트 된 titles.txt는 여기서 찾을 수 있음:
http://wiitdb.com/titles.txt


## 기본 파일 위치

  - 구성 파일:        sd:/usb-loader/config.txt
  - 설정 파일:        sd:/usb-loader/settings.cfg
  - 배경 이미지:      sd:/usb-loader/background.png
  - 커버들:
    - 2D:             sd:/usb-loader/covers/2d/*.png
    - 3D:             sd:/usb-loader/covers/3d/*.png
    - 디스크:         sd:/usb-loader/covers/disc/*.png
    - 모두 (긜고 HQ): sd:/usb-loader/covers/full/*.png
    - 캐쉬:           sd:/usb-loader/covers/cache/*.ccc
  - 타이틀 파일:      sd:/usb-loader/titles.txt
  - 테마:             sd:/usb-loader/themes/THEME_NAME/theme.txt
  - 테마 미리보기:    sd:/usp-loader/themes/*.jpg

  - 오카리나 치트 코드들은 아래 경로에서 찾을 수 있음:
    sd:/usb-loader/codes/*.gct
    sd:/data/gecko/codes/*.gct
    sd:/codes/*.gct
    
  - 오카리나 TXT 치트 코드들은 아래 위치를 사용함:
    - 다운로드 대상:  sd:/usb-loader/codes/*.txt
    - 저장된 .gct  :  sd:/usb-loader/codes/*.gct

  - wiitdb:           sd:/usb-loader/wiitdb.zip
  - 재생 이력:        sd:/usb-loader/playstats.txt

  - .wip 파일들:      sd:/usb-loader/GAMEID.wip
  - .bca 파일들:      sd:/usb-loader/GAMEID.bca
  - .wdm 파일들:      sd:/usb-loader/GAMEID.wdm

  - nand 이미지       usb:/nand

  - FAT/NTFS 상의 게임들
	                    usb:/wbfs/GAMEID.wbfs
  	또는:             usb:/wbfs/TITLE [GAMEID].wbfs
  	또는:             usb:/wbfs/GAMEID_TITLE/GAMEID.wbfs
  	또는:             usb:/wbfs/TITLE [GAMEID]/GAMEID.wbfs
  	(또는 usb:/ 대신에 sd:/)

이것들은 기본 위치이며 배경과 커버는 구성 가능합니다.
설정 파일이 sd:/usb-loader에서 발견되지 않으면, sd:/apps/USBLoader/config.txt
(또는 홈브류 채널에서 시작하는 데 사용되는 디렉토리)를 검색하고, 발견되면
기본 경로는 다음과 같습니다. 해당 위치로 설정하십시오.

글로벌 설정 파일 sd:/usb-loader/config.txt 외에 apps 폴더의 config.txt도 사용됩니다 기본적으로:
sd:/apps/USBLoader/config.txt 이지만 로더가 홈브류 채널에서 시작된 위치에 따라 다릅니다.

구성 파일을 지정하는 또 다른 방법은 추가 인수를 허용하는 PC의 
wiiload 유틸리티를 사용하는 것 입니다:
C:\> wiiload usbloader.dol config21.txt
sd:/usb-loader/config21.txt를 불러오고
configl 옵션을 전달할 수도 있습니다:
C:\> wiiload usbloader.dol video=ntsc

따라서 시작 위치에 따라 다른 구성을 가질 수 있습니다.
이는 포워더에서 시작된 로더를 simple / childproff로 구성하고 홈브류 채널에서 시작하여
설치 및 제거 옵션을 포함하도록 구성 할 수 있으므로 유용 할 수 있습니다
이를 위해, sd:/apps/USBLoader/를 sd:/apps/USBLoader_admin으로 복사 한 다음
sd:/apps/USBLoader/config.txt에 simple = 1로 설정하고 sd:/apps/USBLoader_admin/meta를
편집 (또는 삭제) 합니다. .xml을 사용하여 다른 이름을 표시합니다.


## 구성 및 커버 용 USB FAT

SD 카드가 먼저 config.txt를 검색하고 찾을 수 없다면 FAT 파티션이있는 USB HDD가
usb:/로 마운트되고 config.txt를 검색합니다.
이 경우 위에서 언급 한 모든 경로는 sd:/ 대신에 usb:/.
구성 및 커버에 USB FAT를 사용하면 커버를 더 빨리 장착 할 수 있습니다.
(일반적으로 USB HDD 장치는 SD 카드보다 빠릅니다)
SD 카드에서 응용 프로그램을 불러오지만 구성 및 커버에 USB를 사용하려면 inSDroot의
모든 내용을 USB FAT 파티션으로 복사하지만, inSDroot / apps 디렉토리 만 SD 카드에 복사하고
sd:/apps/USBLoader/config.txt 및 sd:/usb-loader/config.txt를 삭제합니다.

참고: SD 또는 USB 엄지 드라이브에 2 개의 파티션을 생성하려면 gparted와 
같은 특별한 도구를 사용해야합니다: http://gparted.sourceforge.net/
2 개의 주 파티션을 만들고 FAT32로 포맷 한 다음 두 번째 파티션을 WBFS로 다시 포맷합니다.
구성 및 커버 용으로 200MB, WBFS 용으로 나머지 200MB의 경우 권장되는 파티션 크기.

참고: FAT 파티션에 접근하는 데 문제가 있다면 윈도우 파티션 편집기에서 'active'으로 표시되어
있는지 확인합니다. (또는 gparted를 사용하는 경우 파티션을 'boot'플래그로 표시합니다.)


제한:
- USB FAT는 SD에서 config.txt를 찾을 수 없는 경우에만 마운트됩니다.


테마:
-------

로더를 사용자 정의하는 또 다른 방법은 테마를 사용하는 것입니다.
테마는 다음 위치에 구성 파일을 작성하여 정의:
sd:/usb-loader/themes/THEME_NAME/theme.txt
그리고 배경 이미지:
sd:/usb-loader/themes/THEME_NAME/background.png
sd:/usb-loader/themes/THEME_NAME/background_wide.png

theme.txt에서 사용할 수있는 옵션은 아래에 설명되어 있고,
기본적으로 보기를 정의하는 옵션 만 허용되며 그 외 모든 것은 theme.txt에서 무시됩니다.
배경 이미지 (background.png 또는 배경 옵션)은 테마 폴더(sd:/usb-loader/themes/THEME_NAME/)에서
먼저 검색되고 찾지 못하면 기본 폴더(sd:/usb-loader/)에서 검색됩니다.

다른 테마 GUI 리소스:
  favorite.png
  pointer.png
  hourglass.png
  font_uni.png (새로운 유형의 512 문자 유니 코드)
  font.png (오래된 유형 128 문자 아스키 코드)
  font_clock.png
  window.png, page.png
  button.png, radio.png, checkbox.png
배경 이미지와 동일한 검색 방법이이 파일에 적용됩니다.
usb-loader/resources에 몇 가지 예제 파일이 있지만 프로그램이 해당 위치에서 검색하지 않고, 사용할 기본 또는 테마 폴더에 복사해야 합니다.

배경 오버레이 지원:
배경 위에 오버레이 될 추가 이미지를 제공 할 수 있습니다:
 - 콘솔 배경에 대한 bg_overlay.png 또는 bg_overlay_w.png
 - GUI 배경의 경우 bg_gui_over.png 또는 bg_gui_over_w.png
*_w.png 변형이 발견되지 않으면 정상 사용됩니다.
테마가 사용되면 기본 폴더가 아닌 테마 폴더에서만 오버레이 파일이 검색됩니다.

배경 이미지의 자동 크기 조정:
버전 41 배경 너비는 640보다 클 수 있으므로 둘 중 하나가됩니다.
 - 와이드 스크린 경우 축소됩니다.
 - 와이드 스크린 아닌 경우 잘립니다.
640x480까지 내려갑니다. 참고 : 높이는 여전히 480이어야 합니다.

GUI 버튼, 아이콘 및 창 테마 이미지:
버튼 이미지: button.png, radio.png, checkbox.png
윈도우 이미지: window.png, page.png
States: 버튼 이미지에는 단일 버튼 이미지가 포함될 수 있거나
여러 이미지를 여러 상태로 표시할 수 있습니다:
- normal, flash, hover, press, press hover, inactive
임의의 수의 버튼이 있을 수 있고, 누락 된 상태가 생성되면 정상 상태 + 색상 표시 및 효과가 사용됩니다.
버튼 폭:높이는 2:1이어야 상태의 수를 계산할 수 있습니다. 계산 = 높이*2/너비
크기 조정 : 버튼이 수평으로 3 개의 영역으로 나뉩니다 : 1/4 1/1/2 1/4
그리고 마지막은 중간에 필요한만큼 줄이면서 비례 적으로 비례합니다.
라운드 버튼은 처음과 마지막 부분 만 사용합니다.
마찬가지로 창 이미지는 수직으로 3 개의 영역으로 나뉘며 동일한 규칙이 적용됩니다.
이미지 너비와 높이는 4로 나눌 수 있어야합니다.


GUI 모드:
---------

기본적으로 콘솔 모드가 시작됩니다.
GUI 모드로 전환하려면 기본 화면에서 B 버튼을 누릅니다.
GUI 모드에서는 기본적으로 다음 버튼이 사용됩니다 (다시 매핑 할 수 있음):
    A 버튼 : 선택된 게임 시작
    B 버튼 : 콘솔 모드 돌아가기
    왼쪽/오른쪽 버튼 (그리드): 이전/다음 페이지
    왼쪽/오른쪽 버튼 (커버플로우) : 다음 커버로 회전 - 계속 누르고 있으면 빠르게 회전합니다.
    위쪽/아래쪽 버튼 (그리드) : 행 (1-3)의 수 전환
    아래쪽 버튼 (커버플로우) : 센터 커버를 뒤쪽/앞쪽 뒤집는다.
    아래쪽 버튼 : GUI 스타일 변경 (그리드 -> 플로우 -> 플로우-z -> 커버플로우 3d -> 기타)
    버튼 1, +, - : 옵션, 설치, 삭제
    버튼 2: 즐겨찾기 게임 목록
    홈 버튼 : 종료
GUI 모드에 배경 이미지는 파일에서 변경할 수 있음:
    sd:/usb-loader/themes/Theme_Name/bg_gui.png  또는
    sd:/usb-loader/bg_gui.png


## 커버 다운로드

커버는 모든 게임에 대해 한 번 또는 게임 단위로 다운로드 할 수 있습니다.
모든 게임의 커버를 다운로드하려면 글로벌 옵션 화면으로 이동하여 
"<Download All Covers>"로 이동 한 다음 오른쪽 또는 왼쪽 버튼을 누릅니다.
왼쪽과 오른쪽 버튼에는 차이가 있음:
- 오른쪽 버튼을 누르면 모든 누락된 커버가 다운로드됩니다.
- 왼쪽 버튼은 이미 존재하는 것을 포함하여 모든 커버를 다운로드합니다.
현재 선택된 게임에 대한 표지를 다운로드하려면 게임 옵션 화면으로 이동하여 "Cover Image:" 옵션으로 이동 한 다음 오른쪽 또는 왼쪽을 누릅니다.
오른쪽 버튼과 왼쪽 버튼의 같은 차이가 다운로드 전체 커버와 마찬가지로 여기에 적용됩니다.
커버를 다운로드하는 방법은 구성 옵션 download_* 와 url_*을 사용하여 추가로 사용자 정의 할 수 있습니다.
아래의 옵션에 대한 문서는 구성 파일 섹션에서 참조합니다.

## 자녀 보호 및 관리자 기능 잠금 해제

로더가 제한된 기능으로 구성된 경우 암호로 잠금을 해제 할 수 있습니다
- "secret" wiimote 버튼 조합. 제한된 기능이란 일반적으로 "자녀 보호"에 사용되는
"simple" 또는 "disable_*" 또는 "hide_game"옵션 중 하나를 의미합니다.

관리자 모드가 잠금 해제되면 이전에 잠긴 모든 기능에 액세스 할 수 있습니다. 
또한 잠금 해제되면 hide_game 옵션으로 숨겨진 모든 게임이 표시됩니다.

잠금 해제 화면에 액세스하려면 1 버튼을 5 초 동안 누르고 있으면 화면이 나타납니다.
"Enter Code :"텍스트를 본 다음 위모트 버튼을 올바른 순서로 누릅니다.
성공하면 SUCCESS라는 단어가 화면에 나타납니다. 그렇지 않으면 단어 LOCKED! 나타납니다.
잠금 해제 화면에는 30 초 제한 시간이 있기 때문에 올바르지 않은 암호를 입력하면 자동으로 잠깁니다.
원래 설정대로 잠금을 다시 설정하려면 1 버튼을 5 초 동안 누르고 있으면 잠금 장치가 자동으로 켜집니다.
로더가 시작되면 잠금이 항상 사용 가능하게됩니다.

이 기능은 admin_unlock = [1], 0 옵션으로 제어됩니다.
기본적으로 사용 가능합니다. 관리 모드의 잠금을 해제하는 기능을 비활성화하려면
다음 옵션을 설정합니다. admin_unlock = 0

기본 관리자 잠금 비밀번호는 다음과 같습니다 : BUDAH12
이를 변경하려면, 구성 옵션을 사용합니다. : unlock_password = [BUDAH12]
암호 길이는 10 문자로 제한됩니다. 암호 주위에 따옴표를 사용하지 않습니다. 원하는 것을 입력합니다.
예.  unlock_password = 12UDAB
다음은 비밀번호에 대한 문자 매핑 버튼입니다.:
      D-패드 위쪽:   U
      D-패드 아래:   D
      D-패드 오른쪽: R
      D-패드 왼쪽:   L
      B 버튼:        B
      A 버튼:        A
      마이너스 버튼: M
      플러스 버튼:   P
      홈 버튼:       H
      1 버튼:        1
      2 버튼:        2

특정 게임을 숨기려면 게임 옵션 화면을 사용하고 "Hide Game" 설정을 전환합니다.
이렇게하면 관리자 모드가 잠겨있을 때 숨겨져있는 게임을 설정할 수 있습니다.
이 옵션을 보려면 admin_unlock을 활성화해야합니다 (기본값). 관리자 모드는 잠금 해제 상태 여야합니다!
- 참조: 이 기능은 config.txt의 hide_game 옵션을 완전히 대체하지만 함께 사용할 수 있습니다.
        현재 hide_game에 나열된 게임은 잠금 해제되어있을 때 표시되지만 게임 옵션에서는 기본적으로
        숨김으로 표시되며 config.txt에서 제거하지 않으면 숨김 상태로 변경할 수 없습니다.
- 참조2: hide_game에있는 모든 게임을이 새로운 기능으로 변환하는 쉬운 방법은 config.txt에 hide_game을 
        사용하여 로더를 시작한 다음, 게임에서 게임 옵션으로 이동하여 (먼저 관리자 잠금을 해제해야 할 수 있음) 
	    무언가를 변경하고 저장합니다. 모든 hide_game 항목이 자동으로 저장됩니다. 
        그런 다음 hide_game 항목을 config.txt에서 완전히 제거 할 수 있습니다.


## 다양한 컨트롤러 버튼 맵핑
컨트롤러 맵핑과 함께 나열된 17개의 가능한 버튼이 있습니다.

	--------------------------------------------------------------
	버튼       위모트     클래식    게임큐브    기타       눈챠크
	--------------------------------------------------------------
	위쪽       위쪽       위쪽       위쪽       STRUM UP
	오른쪽     오른쪽     오른쪽     오른쪽     없음
	아래쪽     아래쪽     아래쪽     아래쪽     STRUM DOWN
	왼쪽       왼쪽       왼쪽       왼쪽       없음
	-          -          -                     -
	+          +          +                     +
	A          A          A          A          초록        
	B          B          B          B          빨강          
	홈         홈         홈         시작    
	1          1                          
	2          2                          
	X                     X          X          파랑
	Y                     Y          Y          노랑
	Z                     ZL/ZR      Z          주황        Z
	C                                           C
	L                     L          L
	R                     R          R

버튼의 동작은 button_* 옵션을 통해 변경할 수 있습니다.

## 타이틀 변경

게임 타이틀 이름을 바꾸려면 SD에서 파일을 편집합니다.
sd:/usb-loader/titles.txt 또는 sd:/usb-loader/custom-titles.txt
형식은:
GAMEID = 게임 타이틀
예제:
RSPP = Wii Sports

## 구성 파일

	# "#"로 시작하는 줄은 주석입니다.
	# 기본값은 [ ]입니다.
	#
	# 옵션의 카테고리는 2가지 : 글로벌 및 테마
	#   테마 옵션 (theme.txt) 보이는 것에만 영향을 주지만, 다른 모든 것은 무시됩니다.
	#   글로벌 옵션 (config.txt) 테아 옵션을 포함한 모든 옵션을 수락합니다.
	#
	#
	# 테마 옵션:
	# ==============
	#
	# background = [background.png]
	# wbackground = [background_wide.png]
	#   배경 이미지에 사용할 파일.
	#   파일은 (sd:/somedir/myimage.png 같은) 절대 경로가 될 수 있습니다.
	#   지정된 배경이 절대 경로가 아닌 경우 테마 폴더(sd:/usb-loader/themes/THEME_NAME/)
	#   및 기본 디렉토리 (sd:/usb-loader)에서 검색됩니다.
	#
	# background_base = [background.png]
	# wbackground_base = [background_wide.png]
	#   bg_overlay* 파일이 오버레이되는 기본 배경 이미지.
	#   실제로이 옵션은 일반 배경 옵션과 동일하지만 유일한 차이는 중첩된 배경을
	#   지원하는 버전에서 이해되므로 앞으로 및 이전 버전과 호환되는 테마를 만들 수 있습니다.
	#
	# background_gui = [bg_gui.png]
	# wbackground_gui = [bg_gui_wide.png]
	#  GUI 모드 배경 파일.
	#
	# layout = original2 original small medium large large2 [large3],
	#          ultimate1 ultimate2 ultimate3 kosaic
	#   original:   6 라인 (wanikoko 1.0-1.1)
	#   original2: 12 라인 (wanikoko 1.2-1.5)
	#   small:      9 라인 (원래와 같은 배경)
	#   medium:    17 라인
	#   large:     21 라인 (nixx)
	#   large2:    21 라인 (usptactical)
	#   large3:    21 라인 (oggzee) 
	#   ultimate1: 12 라인 (WiiShizza)
	#   ultimate2: 12 라인 (jservs7 / hungyip84)
	#   ultimate3: 12 라인 (WiiShizza - 오른쪽 커버)
	#
	#
	# covers = [1], 0
	#   (커버 활성화/비활성화)
	#
	# console_coords = x,y,width,height
	# wconsole_coords = x,y,w,h (widescreen)
	#
	# console_color = foreground,background
	#   (색상값: 0-15)
	#   어두움:  0=검은색, 1=빨간색, 2=초록색, 3=노란색, 4=파란색, 5=보라색, 6=청록색, 7=밝은 회색
	#   밝음: 8=회색, 9=빨간색, 10=초록색, 11=노란색, 12=파란색, 13=보라색, 14=청록색, 15=흰색
	#   참조: http://www.silverpoint.com/leo/color/c-16.gif (상단 0에서 하단 15)
	#
	# covers_coords = x,y
	# wcovers_coords = x,y (widescreen)
	#
	# hide_header = [0],1 
	# hide_hddinfo = 0,[1]
	# hide_footer = [0],1 
	#   이 옵션은 기본 메뉴의 모양을 제어합니다.
	#
	# simple = [0], 1
	#   테마의 단순 옵션을 사용하면 hide_footer 옵션에만 영향을 미치며 disable_* 옵션은 변경되지 않습니다.
	#   글로벌 config.txt의 simple 옵션을 사용하여 disable_* 옵션도 변경합니다.
	#
	# colors = [dark], bright, mono
	#   dark나 bright 배경을 위해 prefedines 색상 세트를 선택하거나
	#   mono가 지정되면 일반 2 색상 텍스트를 선택합니다.
	#
	# color_header, color_selected_fg, color_selected_bg,
	# color_inactive, color_footer, color_help
	#   개별 텍스트 색상을 설정합니다. 값은 0-15입니다.
	#
	# cover_style = [standard], 3d, disc
	#   3D 커버 및 디스크 커버 지원
	#   이 옵션은 어느 cover_url 및 cover_path가 사용되는지 선택합니다.
	#
	# console_transparent = [0], 1
	#   투명한 콘솔을 사용합니다.
	#
	# covers_size = width, height
	#   기본값: covers_size = 160, 225
	#   불러온 이미지가 다른 크기 인 경우 지정된 크기가 됩니다.
	#
	# wcovers_size = width, height
	#   기본값: wcovers_size = 130, 225
	#   와이드 스크린 설정에 사용됩니다. 설정하지 않으면 covers_size를 사용하고 와이드 스크린 크기로 적절하게 조정합니다.
	#
	# cursor = ">>"
	#   커서 모양을 최대 2 문자로 변경합니다. 비어있을 수 있습니다.
	#   공백을 원한다면 메뉴가 이동되지 않도록 다음과 같이 따옴표를 사용합니다: cursor = " "
	#
	# menu_plus  = "[+] "
	#   기본, 옵션 및 시작 메뉴에서 [+] 표시를 변경합니다.
	#   최대 4 문자를 사용합니다.
	#
	# gui_text_color = [black], white, RRGGBBAA
	#   GUI 모드에서 텍스트 색상 설정
	#   참고: 검정색 또는 흰색 이외의 색상을 사용하려면 다음 구성 요소가있는 16 진수 값으로 나타내야합니다: RRGGBBAA
	#   RR=빨간색, GG=초록색, BB=파란색, AA=알파
	#   예제: 빨간색 = FF0000FF, 파란색 = 00FF00FF, 노란색 = 00FFFFFF
	#
	# gui_text_outline = [FF], AA, RRGGBBAA, black, white
	# gui_text_shadow = [00], AA, RRGGBBAA, black, white
	#   GUI 모드에서 텍스트의 윤곽선과 음영 색 알파 만 지정되면
	#   텍스트 색이 밝은 지 또는 어두운 지에 따라 윤곽선/음영색을 검정색 또는 흰색으로 설정합니다.
	#
	# gui_text2_color = [white], black, RRGGBBAA
	# gui_text2_outline = [FF], AA, RRGGBBAA, black, white
	# gui_text2_shadow = [00], AA, RRGGBBAA, black, white
	#   배경이 어두운 커버 플로우 모드의 텍스트 색상
	#
	# gui_title_top = [0], 1
	#   1이면 GUI 텍스트가 표지 위에 나타납니다. 0이면 아래에 있습니다.
	#
	# coverflow_reflection = color_top, color_bottom
	#   색상은 16 진수 rgba입니다. 0,0은 반사를 비활성화합니다.
	#   기본값: coverflow_reflection = 666666FF, AAAAAA33 
	#
	# gui_cover_area = x, y, w, h
	#   기본값: gui_cover_area = 20, 24, 600, 408
	#   최소 허용 w, h: 480, 320
	#   디버그를 사용하면 영역 사각형이 그려집니다.
	#
	# gui_title_area = x, y, w, h
	#   기본값: 0,0,0,0 의미, 위치는 gui_title_top에 따라 다릅니다.
	#   최소 허용 w, h: 320, 10 참고: h는 아직 사용되지 않습니다.
	#
	# gui_clock_pos = x, y
	#   기본값: -1, -1이라는 의미는 설정 한 시계가 항상 표시되면 제목 위치가 시계 위치로 사용됩니다.
	#
	# gui_page_pos = x, y
	#   기본값: -1, -1의 의미는, 타이틀 위치는 페이지 인디케이터의 위치를 지정합니다.
	#
	# preview_coords = x,y,width,height
	# wpreview_coords = x,y,width,height   (widescreen)
	#   테마 미리보기 이미지의 설정.
	#   X 및/또는 Y를 -1로 설정하면 커버 X 및/또는 Y 위치가 사용됩니다.
	#   올바른 가로 세로 비율을 유지하려면 W 또는 H (또는 둘 다)를 0으로 설정해야합니다.
	#   둘 다 0으로 설정하면 커버 너비가 사용되며 그에 따라 높이가 조정됩니다.
	#
	# home = [reboot], exit, hbc, screenshot, priiloader, wii_menu, 
	#        <magic word>, <channel ID>
	#   메뉴에서 종료 버튼 (일반적으로 홈)을 누르면 수행 할 작업
	#   또한 GUI 및 게임 목록에서 button_H의 작업을 변경합니다.
	#   <magic word>는 Priiloader를위한 4 문자 마법 단어입니다.
	#   <Channel ID>는 대문자로 시작하는 4 문자의 채널 ID입니다
	#   home=screenshot이면 스크린 샷을 만들기 위해 집을 1 초 동안 유지해야합니다. 그렇지 않으면 HBC로 끝납니다.
	#
	# buttons=[options_1], options_B, original
	#   (변경 버튼은 GUI 및 게임 목록의 레이아웃을 제어합니다.)
	#
	#   버튼 레이아웃 "options_1"은 다음과 같습니다.:
	#       B 버튼 - GUI 모드
	#       1 버튼 - 옵션 메뉴
	#
	#   버튼 레이아웃 "options_B"은 다음과 같습니다.:
	#       B 버튼 - 옵션 메뉴
	#       1 버튼 - GUI 모드
	#
	#   버튼 레이아웃 "원본"은 더 이상 사용되지 않지만:
	#       1 버튼 - 옵션 메뉴
	#       B 버튼 - 아무것도 안함
	#
	# button_B = [gui], <other actions>, <magic word>, <channel ID>
	# button_- = [main_menu], <other actions>, <magic word>, <channel ID>
	# button_+ = [install], <other actions>, <magic word>, <channel ID>
	# button_H = [reboot], <other actions>, <magic word>, <channel ID>
	# button_1 = [options], <other actions>, <magic word>, <channel ID>
	# button_2 = [favorites], <other actions>, <magic word>, <channel ID>
	# button_X = A, B, 1, [2], H, -, +, <action>, <magic word>, <channel ID>
	# button_Y = A, B, [1], 2, H, -, +, <action>, <magic word>, <channel ID>
	# button_Z = A, [B], 1, 2, H, -, +, <action>, <magic word>, <channel ID>
	# button_C = [A], B, 1, 2, H, -, +, <action>, <magic word>, <channel ID>
	# button_L = A, B, 1, 2, H, [-], +, <action>, <magic word>, <channel ID>
	# button_R = A, B, 1, 2, H, -, [+], <action>, <magic word>, <channel ID>
	#   이 버튼은 게임 목록 및 GUI의 다음 작업 중 하나에 매핑 될 수 있습니다:
	#     nothing    # 아무것도 안함
	#     options    # 게임 옵션 접속
	#     gui        # GUI 로/에서 전환
	#     reboot     # 시스템 메뉴 재부팅
	#     exit       # 실행중인 응용 프로그램 종료
	#     hbc        # 홈브류 채너 종료
	#     screenshot # 스크린샷
	#     install    # 게임 설치
	#     remove     # 게임 삭제
	#     main_menu  # 메인 메뉴 접속 
	#     global_ops # 글로벌 옵션 메뉴 접속
	#     favorites  # 즐겨찾기 보기 토글
	#     boot_game  # 드라이브에서 게임 부팅
	#     boot_disc  # 디스크에서 게임 부팅
	#     theme      # 다음 테마 전환
	#     profile    # 다음 프로파일 전환
	#     unlock     # 잠금 해제 암호 대화 상자에 즉시 접속
	#     sort       # 다음 분류 전환
	#     filter     # 필터 메뉴 접속
	#     priiloader # 마법 단어 Daco를 통해 Priiloader에 접속
	#     wii_menu   # Priiloader가 마법 단어 Pune을 통해 Wii 메뉴를 실행.
	#     <magic word> # 는 Priiloader를 위한 4 문자 마법 단어입니다.
	#     <Channel ID> # 는 대문자로 시작하는 4 문자의 채널 ID입니다.
	#   Wiimote(A, B, 1, 2, -, +, 홈)의 버튼 중 하나를 에뮬레이트하기 위해 X, Y, Z, C, L & R을 선택적으로 타겟팅 할 수 있습니다.
	#   이 에뮬레이션은 모든 곳에서 작동합니다.
	#
	# button_cancel = [B], <comma separated list of buttons>
	#   메뉴에서 뒤로가기 버튼으로 사용할 버튼을 설정합니다.
	#   목록의 유효한 버튼 값은 다음과 같습니다: 
	#     B, 1, 2, -, M, Minus, +, P, Plus, H, Home, X, Y, Z, C, L, R
	#
	# button_exit = [Home], <comma separated list of buttons>
	#   메뉴에서 'home'액션을 수행 할 버튼을 설정합니다.
	#   목록의 유효한 버튼 값은 다음과 같습니다: 
	#     B, 1, 2, -, M, Minus, +, P, Plus, H, Home, X, Y, Z, C, L, R
	#
	# button_other = [1], <comma separated list of buttons>
	#   메뉴에서 다른 동작 또는 대체 동작을 수행 할 버튼을 설정합니다.
	#   여기에는 옵션과 전역 옵션 사이의 전환, 설치 중 BCA 다운로드 선택, 업그레이드 중 meta.xml 무시 등이 포함됩니다.
	#   목록의 유효한 버튼 값은 다음과 같습니다: 
	#     B, 1, 2, -, M, Minus, +, P, Plus, H, Home, X, Y, Z, C, L, R
	#   
	# button_save = [2], <comma separated list of buttons>
	#   메뉴에서 저장 작업을 수행 할 버튼을 설정합니다.
	#   목록의 유효한 버튼 값은 다음과 같습니다: 
	#     B, 1, 2, -, M, Minus, +, P, Plus, H, Home, X, Y, Z, C, L, R
	# 
	# gui_window_color_base = RRGGBBAA 기본값: FFFFFF80
	# gui_window_color_popup = RRGGBBAA 기본값: FFFFFFB0
	#
	# gui_text_color_menu = COLOR / OUTLINE / SHADOW
	# gui_text_color_info = COLOR / OUTLINE / SHADOW
	# gui_text_color_title = COLOR / OUTLINE / SHADOW
	# gui_text_color_button = COLOR / OUTLINE / SHADOW
	# gui_text_color_radio = COLOR / OUTLINE / SHADOW
	# gui_text_color_checkbox = COLOR / OUTLINE / SHADOW
	#   default:
	#   gui_text_color_menu = white / A0 / 44444444
	#   gui_text_color_info = white / A0
	#   각 구성 요소는 "검은 색", "흰색" 또는 RRGGBBAA
	#   OUTLINE 및 SHADOW는 선택 사항입니다.
	#   gui_text_color_menu를 설정하면 info를 제외한 모든 색상이 설정됩니다.
	#   gui_text_color_button을 설정하면 라디오와 체크 박스가 설정됩니다.
	#
	# gui_button_NAME = X, Y, W, H, TextColor, image.png, Type, HoverZoom
	#   NAME은 다음과 같을 수 있습니다: main settings quit style view sort filter favorites jump
	#   TextColor는 gui_text_color_menu와 같은 형식입니다.
	#   (텍스트 색상을 0으로 설정하면 아이콘을 사용할 경우 버튼의 텍스트가 비활성화됩니다.)
	#   Type: 버튼 또는 아이콘
	#   HoverZoom: 0-50 %
	#   좌표 뒤의 매개 변수는 선택적입니다. 기본값:
	#   gui_button_NAME = X, Y, W, H, white/A0/44444444, button.png, button, 10
	#
	# gui_bar = 0, [1], top, bottom
	#   GUI 바를 비활성화 / 활성화하거나 상단 또는 하단 만 활성화합니다.
	#
	# 글로벌 옵션:
	# ===============
	#
	# gui = 0, 1, 2, 3, [4], start
	#   gui = 0 : GUI 비활성화
	#   gui = 1 : GUI 활성화, GUI 메뉴 비활성화, 콘솔 모드 시작
	#   gui = 2 : GUI 활성화, GUI 메뉴 비활성화, GUI 모드 시작
	#   gui = 3 : GUI 메뉴 활성화, 콘솔 모드 시작
	#   gui = 4 : GUI 메뉴 활성화, GUI 모드 시작
	#   gui = start : gui = 4 와 같음
	#
	# gui_transition = [scroll], fade
	#   콘솔과 GUI 모드 간의 GUI 전환 효과 설정
	#
	# gui_style = [grid], flow, flow-z, coverflow3d, coverflow2d, frontrow, vertical, carousel
	#   기본 GUI 스타일 설정
	#
	# gui_rows = [2] (Valid values: 1-4)
	#   GUI 모드에서 기본 행 수 설정
	#
	# gui_lock = [0], 1
	#   위쪽/아래쪽 버튼으로 GUI 스타일 변경 비활성화
	#
	# gui_antialias = [4] {0-4}
	#   커버 플로우 모드 안티 알리아스 레벨 조정
	#
	# gui_pointer_scroll = 0, [1]
	#   게임 목록의 포인터 스크롤을 활성화/비활성화
	#
	# theme = Theme_Name
	#   sd:/usb-loader/themes/Theme_Name/theme.txt에서 지정된 테마 불러오기
	#   참고: 테마는 모든 테마 관련 옵션을 재설정하므로 모든 테마 옵션을
	#   덮어 쓰려면 'theme ='옵션 다음의 행에서 합니다.
	#
	# covers_path = [sd:/usb-loader/covers]
	#   covers_path를 변경하면 다음과 같이 covers_path_*가 모두 바뀝니다: 
	# covers_path_2d = covers_path/2d
	# covers_path_3d = covers_path/3d
	# covers_path_disc = covers_path/disc
	# covers_path_full = covers_path/full
	#   2D/3D/디스크/전체 경로에서 정밀한 제어가 필요한 경우 covers_path 다음에 covers_path_* 옵션을 사용합니다.
	#
	# URL 옵션:
	#   URL에는 다음 태그 중 하나가 포함될 수 있으며 적절한 태그로 대체됩니다:
	#   {REGION}, {WIDTH}, {HEIGHT}, {ID3}, {ID4}, {ID6}, {ID}, {CC}, {PUB}, {ID}
	#   ID6, ID4 및 ID3을 시도하여 올바른 ID를 자동으로 찾습니다.
	#   참고: {WIDTH} 및 {HEIGHT}은 download_all_styles가 ID의 마지막 두 자리 숫자의 {PUB}을
	#   사용하고 다른 지역의 표지를 얻는 데 사용될 수 있으면 제대로 작동하지 않습니다.
	#   예, {ID6}을 {ID3} P {PUB}로 바꿔 PAL 표지를 찾습니다.
	#
	#   cover_url_* 옵션에 대해 여러 개의 URL을 지정할 수 있습니다.
	#   그것들은 공백으로 분리 된 같은 줄에있을 수 있습니다. 예제:
	#   cover_url = http://site1.com/{ID}.png http://site2.org/{ID}.png
	#   또는 여러 줄에서 = 대신 =+를 사용합니다, 예제:
	#   cover_url = http://site1.com/{ID}.png
	#   cover_url =+ http://site2.org/{ID}.png
	#   cover_url =+ http://site3.net/{ID}.png
	#
	# 일반 4 : 3 모드 종횡비 URL 옵션:
	# cover_url = URL      (기본 2D 평면 커버 url)
	# cover_url_3d = URL   (3D 커버 url)
	# cover_url_disc = URL (디스크 커버 url)
	# cover_url_full = URL (전체 커버 url)
	# cover_url_hq = URL   (HQ 전체 커버 url)
	#
	#   기본:
	#
	#   cover_url = http://wiitdb.com/wiitdb/artwork/cover/{CC}/{ID6}.png
	#
	#   cover_url_3d = http://wiitdb.com/wiitdb/artwork/cover3D/{CC}/{ID6}.png
	#
	#   cover_url_disc =
	#   cover_url_disc =+ http://wiitdb.com/wiitdb/artwork/disc/{CC}/{ID6}.png
	#   cover_url_disc =+ http://wiitdb.com/wiitdb/artwork/disccustom/{CC}/{ID6}.png
	#
	#   cover_url_full = http://wiitdb.com/wiitdb/artwork/coverfull/{CC}/{ID6}.png
	#
	#   cover_url_hq = http://wiitdb.com/wiitdb/artwork/coverfullHQ/{CC}/{ID6}.png
	#
	# download_id_len = 4, [6]
	#   저장된 파일 이름에 대해 다운로드 한 표지 ID 길이를 지정
	#
	# download_all_styles = [1], 0
	#   모든 표지 스타일 (플랫, 3D, 디스크) 또는 현재 스타일 만 다운로드
	#
	# download_cc_pal = [AUTO], EN, FR, DE, AU, ...
	#   이 코드는 PAL 지역의 {CC} 태그 대신 사용됩니다.
	#   AUTO를 지정하면 콘솔 국가에 따라 코드가 설정됩니다.
	#   오스트레일리아: AU, 브라질: PT 이면, 콘솔 언어가 사용됩니다.
	#   지정된 cc 코드로 이미지를 찾을 수 없으면 다운로드가 EN 코드로 다시 시도됩니다.
	#
	# titles_url = http://wiitdb.com/titles.txt?LANG={DBL}
	#   titles.txt 업데이트 용 Url
	#
	# device = [ask], usb, sdhc
	#   로더를 시작할 때 사용할 장치를 지정합니다.
	#
	# partition = [auto], ask, WBFS1, ...WBFS4, FAT1, ...FAT9, NTFS1, ...NTFS9
	#   로더를 시작할 때 사용할 파티션을 지정합니다.
	#   참고: -222 버전 기본값은 FAT1 입니다.
	#
	# simple = [0], 1
	#   (simple 활성화/비활성화 /아동보호 모드)
	#   simple=1 설정하면 모든 disable_xxx 옵션과 hide_footer가 1로 변경되고 confirm_start가 0으로 변경됩니다.
	#   simple=0 설정하면 반대가 됩니다.
	#   disable_xxx, hide_xxx 및 confirm_start 옵션 중 하나를 개별적으로 설정할 수 있습니다..
	#
	# confirm_start = [1], 0
	#   게임 시작 시 확인이 필요한지 여부를 지정합니다.
	#
	# disable_remove = [0],1
	# disable_install = [0],1
	# disable_options = [0],1
	# disable_format = [0],1
	#   훌륭한 사용 권한 제어
	#
	# admin_unlock = [1], 0.
	#   사용하도록 설정하면 잠금 해제 관리자 모드가 허용되므로 접속할 수 있습니다.
	#   모든 설정에서 해당 simple 또는 disable_* 옵션을 비활성화합니다.
	#   
	# unlock_password = [BUDAH12]
	#   관리자 잠금 비밀번호 설정
	#
	# install_partitions = [only_game], all, 1:1, iso
	#   DVD의 어떤 파티션이 HDD에 설치되는지 제어합니다.
	#   - wbfs 제한으로 인해 여전히 지워지는 마지막 256kb를 제외하고 1:1 비활성화 사용:
	#     wbfs 블록 크기가 Wii 디스크 크기에 맞춰지지 않음
	#   - iso: NTFS에서는 iso 파일에 대한 정확한 덤프를 만듭니다. WBFS/FAT에서는 1:1과 동일하게 동작합니다
	#
	# fat_split_size = [4], 2, 0
	#   분할 선택 4: 4gb-32kb 또는 2: 2gb-32kb 또는 0: 분할 없음 - ntfs 만
	#
	# fat_install_dir = [1], 0, 2, 3
	#   Select install filename layout on fat:
	#   fat_install_dir = 0 /wbfs/GAMEID.wbfs
	#   fat_install_dir = 1 /wbfs/GAMEID_TITLE/GAMEID.wbfs
	#   fat_install_dir = 2 /wbfs/TITLE [GAMEID]/GAMEID.wbfs
	#   fat_install_dir = 3 /wbfs/TITLE [GAMEID].wbfs
	# fs_install_layout은 fat_install_dir의 별칭입니다.
	#
	# ntfs_write = [0], 1, norecover
	#   0은 사용할 수 없으며 1은 ntfs 쓰기 지원을 활성화합니다 
	#   norecover는 쓰기를 가능하게하지만 PC 복구가 선호 될 때 부정확하게 마운트 해제 된 fs를 마운트하는 것을 방지합니다.
	#
	# music = [1], 0, filename, PATH
	#   배경 음악 재생 (단 하나의 옵션 만 지정해야 함)
	#   예제:
	#   music = 1
	#     (기본값) sd:/usb-loader 디렉토리에서 모든 .mp3 또는 .mod 파일 (둘 중 먼저 발견되는 것)을 무작위로 재생합니다
	#   music = sd:/usb-loader/my_music.mp3
	#     my_music.mp3 재생. 파일 이름은 sd:/usb-loader 또는 절대 경로 이름을 기준으로 지정할 수 있습니다.
	#   music = sd:/music
	#     해당 폴더에서 모든 .mp3 또는 .mod 파일을 무작위로 재생합니다.
	#   music = 0
	#     음악을 비활성화 합니다.
	#
	# widescreen = [auto], 0, 1
	#   * 와이드 스크린이 활성화 (또는 자동 감지) 된 경우 다음 옵션이 사용됩니다:
	#      - wbackground
	#      - wbackground_base
	#      - wbackground_gui
	#      - wconsole_coords
	#      - wcovers_coords
	#      - wcovers_size
	#   * 와이드 스크린 모드에서 표지 이미지는 먼저 GAMEID_wide.png라는
	#     이름으로 검색되고 GAMEID.png가 없으면 제대로 크기가 조정됩니다.
	#   * 일부 레이아웃에서는 large3 및 ultimate3과 같은 자동으로
	#     와이드 스크린 cooridinate가 지정되므로 이러한 레이아웃 중 하나를
	#     사용하면 수동으로 지정하지 않아도됩니다.
	#
	# hide_game = [0], GAMEID1, GAMEID2, ...
	#   목록에서 게임 숨기기 (자녀 보호를 위해 사용될 수 있음)
	#   여러 개의 게임을 한 줄에 쉼표 ","로 구분하거나
	#   각 게임을 hide_game = GAMEID 행으로 구분하여 지정할 수 있습니다.
	#   hide_game = 0으로 설정하면 숨기기 목록이 재설정됩니다.
	#   GAMEID는 4 문자의 게임 ID입니다.
	#   예제: hide_game = RZZP, RDCP
	#
	# pref_game = [0], GAMEID1, GAMEID2, ...
	#   목록에 첫 번째로 표시 할 기본 게임입니다.
	#   구문은 hide_game과 같습니다.
	#   예제: pref_game = RHAP, RSSP
	#
	# confirm_ocarina = [0], 1
	#   오카리나를 사용하고 코드를 찾았을 때 확인이 필요한지 여부를 지정합니다.
	#
	# cursor_jump = [0] or N
	#   왼쪽/오른쪽 이동 거리를 설정합니다 (0으로 끝 페이지/다음 페이지 점프를 할 경우).
	#
	# start_favorites = [0], 1
	#   즐겨 찾기 게임 목록으로 시작
	#
	# clock_style = [24], 12, 12am, 0
	#   시계 스타일을 설정합니다. 0은 시계를 비활성화 합니다.
	#
	# sort_ignore = [A,An,The], ...
	#   제목 정렬시 무시해야 할 단어
	#   쉼표로 단어를 구분하고 대괄호는 포함하지 않습니다.
	#   이전 정렬 방법의 경우 sort_ignore=0으로 설정 - 아무 것도 무시하지 않음
	#
	# debug = [0], 1, 8
	#   시작되면 진단 메시지를 표시합니다.
	#   디버그=8 인 벤치 마크 모드 및 게임 시작 또는 설치
	#
	# debug_gecko = [0],1,2,3
	#   usb gecko에 디버그 정보 쓰기 (1=디버그, 2=콘솔, 3=모두)
	#
	# profile_names = [default], name2, name3,...
	#   프로필 - 일명 좋아하는 여러 그룹
	#   (최대 프로필 : 10, 최대 프로필 이름 길이 : 16)
	#   이 옵션을 사용하여 프로필을 추가, 제거 및 재정렬 할 수 있습니다만,
	#   이름을 바꾸려면 settings.cfg에서도 프로필 이름을 변경해야합니다.
	#   그렇지 않으면 다음 번에 설정을 저장하면 이전 이름이 새 이름으로 간주되고
	#   이전 이름은 잊어 버리게됩니다.
	#   프로필은 글로벌 옵션 화면에서 전환 할 수 있습니다.
	#   게임 즐겨 찾기 설정을 변경하는 것은 게임 옵션 화면에서 평상시처럼 완료됩니다.
	#
	# profile = name
	#   사용할 기본 프로필을 지정합니다.
	#   글로벌 설정 저장은 어떤 프로파일이 사용되는지를 저장합니다
	#
	# profile_start_favorites = {[0], 1} ...
	#   즐겨 찾기를 활성화하거나 비활성화 할 때 각 프로필이 전환 될시기를 지정합니다.
	#   profile_start_favorites 0 1 1 1 1 1 1 1 1 1
	# 
	# db_url = [http://wiitdb.com/wiitdb.zip?LANG={DBL}]
	#   데이터베이스를 다운로드 할 URL입니다.
	#
	# db_language = [AUTO], EN, JA, German, etc
	#   {DBL} 태그에 사용할 언어입니다. 유효하지 않거나 로더가
	#   표시할 수 없는 경우이 값은 영어로 기본 설정됩니다.
	#   국가 코드 (EN)와 언어 (영어)가 모두 유효합니다.
	#
	# db_show_info = [1], 0
	#   데이터베이스에서 불러온 정보를 표시합니다.
	#
	# db_ignore_titles = [0], 1
	#   게임 이름을 지정할 때 데이터베이스의 제목을 무시하도록 설정합니다.
	#
	# write_playstats = [1], 0
	#   재생 히스토리 파일에 기록합니다.
	#
	# sort = [title-asc], etc
	#   기본 정렬 방법을 변경합니다. 기본값은 제목 오름차순입니다.
	#
	#   Valid sort options:
	#     "title"         => 타이틀
	#     "players"       => 플레이어 수
	#     "online_players"=> 온라인 플레이어 수
	#     "publisher"     => 퍼블러셔
	#     "developer"     => 개발자
	#     "release"       => 출시일
	#     "play_count"    => 실행 횟수
	#     "install"       => 설치 날짜
	#                        (이것은 FAT 또는 NTFS 드라이브에서만 작동합니다.)
	#     "play_date      => 마지막 실행 날짜
	#
	#   오름차순으로 사용하려면 옵션에 "-asc"를 추가합니다.
	#     즉: sort = players-asc
	#   
	#   내림차순을 사용하려면 옵션에 "-desc"를 추가합니다.
	#     즉: sort = players-desc
	#
	# translation = [AUTO], EN, custom, etc.
	#   현재 자동값: JA, EN, DE, FR, ES, IT, NL, ZH, ZH, KO
	#   해당 파일이 존재하는 한 모든 파일 이름이 지원됩니다. 
	#   번역 파일은 현재 DE, DK, ES, FI, FR, GR, IT, JA, KO, NL, NO, PT_BR, PT_PT, TR, ZH_CN, ZH_CN-clamis, ZH_TW 존재합니다.
	#
	# load_unifont = [0], 1
	#   unifont.dat를로드할지 여부를 지정합니다. unifont.dat에는 번역 또는 wiitdb 정보가 올바르게 표시 될 수 있도록
	#   아시아 언어 지원에 필요한 모든 유니 코드 문자가 포함되어 있습니다.
	#   JA, KO 또는 ZH로 변환이 시작되거나 db 언어가 JA, KO, ZH 인 경우 load_unifont는 자동으로 1로 전환합니다.
	#   참고: LATIN 유니 코드 세트는 이미 로더에 내장되어 있으므로 독일어, 프랑스어, 스페인어 등을 표시 할 수 있습니다.
	#   unifont.dat는 필요하지 않습니다.
	#
	# wiird = [0], 1, 2
	#   1 = 디버거 활성화
	#   2 = 디버거 및 일시 중지 시작 활성화
	#
	# select = [previous], start, middle, end, most, least, random
	#   시작 시 기본적으로 선택되는 게임을 선택합니다.
	#   새로운 기본값은 이전 게임입니다 (이전 작업을하려면 select = start를 설정합니다).
	#   'start', 'middle', 'end'은 목록의 위치를 나타냅니다.
	#   'most'와 'least'는 (Cfg) 재생 수를 의미합니다.
	#   'random'는 매번 다른 게임을 선택합니다.
	#
	# adult_themes = [0], 1
	#   성인용 테마를 다운로드 할 수 있는지 결정합니다.
	#
	# theme_previews = [1], 0
	#   테마 미리보기 이미지를 다운로드하여 표시할지 여부를 결정합니다.
	#
	# return_to_channel = [0], auto, JODI, FDCL, ...
	#   게임이 선택한 채널 ID로 돌아갑니다.
	#   예, HBC의 경우 JODI, Cfg를 다시 불러오는 경우 FDCL 또는 DCFG와 같은 전달자 채널을 사용합니다.
	#   0은 기본 Wii 메뉴 작업입니다
	#   auto: 로더가 시작된 곳에서 채널 ID를 감지하려고 시도합니다.
	#   (일부 포워더는 자동으로 자동 감지되지 않지만 FIX94의 공식 포워더는 자동 감지됩니다.)
	#
	# disable_nsmb_patch = [0],1
	# disable_pop_patch = [0],1
	# disable_dvd_patch = 0,[1]
	#   선택적으로 로더가 수행하는 패치를 비활성화 합니다.
	#
	#   nsmb = 뉴 슈퍼 마리오 브라더스.
	#   pop = 페르시아의 왕자 : 망각의 모래
	#   dvd = Hermes의 디스크 검사 패치.
	#
	#   PoP를 사용하려면 DVD 패치를 비활성화 합니다.
	#   옵션을 비활성화(패치하지 않음)하려면 1로 설정합니다.
	#
	# gamercard_url = URL
	# gamercard_key = key
	#   이러한 옵션은 커버 URL 옵션과 동일하게 작동하며
	#   =+ 연산자를 사용하여 여러 사이트/키를 추가 할 수 있습니다.
	#   키와 URL은 각 순서대로 일치합니다
	#
	#   목록의 키를 0으로 설정하거나 트레일일 키를 생략하면 URL의 각 사이트가 시도되지 않습니다.
	#
	#   URL에 {KEY} 및 {ID6} 태그를 사용할 수 있습니다.
	#
	#   기본값은 WiinnerTag, NCard, DUTag의 순서이지만 빈 키가 있습니다:
	#   gamercard_url =  http://www.wiinnertag.com/wiinnertag_scripts/update_sign.php?key={KEY}&game_id={ID6}
	#   gamercard_url =+ http://www.messageboardchampion.com/ncard/API/?cmd=tdbupdate&key={KEY}&game={ID6}
	#   gamercard_url =+ http://tag.darkumbra.net/{KEY}.update={ID6}
	#   gamercard_key = 0 0 0
	#
	# intro = 0, 1, [2], 3
	#   intro=0 : 검은색 - 직접 게임을 시작할 때만 허용.
	#   intro=1 : 프로그램 이름이 적힌 검은색 배경 (작음)
	#   intro=2 : 컬러 이미지 [기본값]
	#   intro=3 : 회색 이미지
	#   이 옵션은 meta.xml <arguments>에 설정된 경우에만 작동합니다.
	#
	# nand_emu_path = [usb:/nand]
	#   nand 이미지가 위치한 경로를 설정합니다. 그것은 fat??? 드라이브여야 합니다.
	#
	# 게임 호환성 옵션:
	# ===========================
	# 
	# 이 옵션은 글로벌 config.txt에서 설정할 수 있습니다.
	# 옵션은 로더 옵션 화면에서 게임별로 설정할 수 있으며 settings.cfg에 저장됩니다.
	#
	# video = [auto], game, system, pal50, pal60, ntsc
	#   (auto는 게임과 동일합니다.)
	#
	# language = [console], japanese, english, german, french, spanish,
	#            italian, dutch, s.chinese, t.chinese, korean
	#
	# video_patch = [0], 1, all, sneek, sneek+all
	#   'video_patch = 1': 콘솔이 PAL 일 경우 NTSC->PAL 모드를 패치하고 콘솔이 NTSC 인 경우 PAL->NTSC 모드를 패치합니다.
	#   인터레이스/프로그레시브 모드는 변경되지 않습니다.
	#   'video_patch = all' 선택하면 모든 모드가 선택된 비디오 모드로 강제 설정됩니다.
	#   이것은 또한 Wii 설정에서 구성되는 것에 따라 프로그레시브/인터레이스 모드를 강제합니다.
	#   예를 들어 게임이 인터레이스 모드 (MPT)를 사용한다면 프로그레시브 모드를 강제 할 수 있습니다.
	#
	# vidtv = [0], 1
	#   일부 게임에서 필요합니다 (일본어, ...)
	#
	# country_patch = [0], 1
	#   일부 게임과 호환성 향상을 위한 국가 패치
	#
	# fix_002 = [0], 1
	#   이것은 안티 002 수정입니다. 새로운 cIOS(IOS249 rev14 이상)에는 필요하지 않습니다.
	#
	# ios = 247, 248, [249], 222-mload, 223-mload, 224-mload, 222-yal, 223-yal, 250
	#   사용자 정의 IOS 선택
	#   참고: 222-yal은 kwiirk의 cIOS용 입니다.다.
	#   참고: 222-mload는 Hermes의 cIOS 용이며 -222 버전의 기본값입니다.
	#   참고: 사용자 정의 ios로 게임을 시작할 때 몇 초의 지연이 예상됩니다.
	#
	# block_ios_reload = 0, 1, [auto]
	#   일부 게임에서 필요하며, d2x cios와 함께 작동하며 제한된 방법으로 hermes cios에서 작동합니다.
	#   0: 비활성화, 1: 활성화, auto: cios가 d2x이고 버전이 5와 같거나 작으면 활성화
	#
	# alt_dol = [0], 1, sd, disc
	#   (위파워의 네오감마에서)대체 .dol 불러오기 옵션
	#   1 또는 sd로 설정하면 로더 기반 폴더 + GAMEID.dol (4 문자 ID)에서 .dol을 불러옵니다.
	#     [ sd:/usb-loader/GAMEID.dol ]
	#   디스크로 설정하면 wbfs iso 이미지의 .dol 목록이 프롬프트됩니다
	#
	# ocarina = [0], 1
	#   오카리나 - 치트 엔징을 활성화/비활성화
	#
	# hooktype = nohooks, [vbi], wiipad, gcpad, gxdraw, gxflush, ossleep, axframe
	#   오카리나 후크 타입 지정
	#
	# write_playlog = [0], 1, 2, 3
	#   Wii 메시지 게시판 로그에 게임 플레이 통계를 씁니다.
	#   Cfg(예: Priiloader 또는 BootMii 자동 부팅 사용)를 시작하기 전에 Wii 메뉴를 건너 뛰면
	#   이 옵션은 작동하지 않습니다.
	#   0 = 끔, Wii 메시지 보드 로그에 쓰지 않음.
	#   1 = 켬, 해당 언어의 제목이 비어 있거나 영어 제목 또는 일본어 제목(유효한 것)을
	#       사용하지 않는 한, 언어 옵션의 가치에 따라 제목을 설정합니다.
	#   2 = 켬, 타이틀을 일본 타이틀로 설정.
	#   3 = 켬, 타이틀을 영어 타이틀로 설정.
	#   게임 별 메뉴에서 옵션은 각각 "Off", "On", "Japanese Title", "English Title"로 표시됩니다.
	#
	# clear_patches = [0],1,all
	#   (1) return_to_channel 이면 DVD 검사는 비활성화됩니다.
	#   'all'이면 모든 .dol 패치가 비활성화됩니다.

## 구성 파일 샘플

    # USBLoader config
    # lines starting with # are comments
    # see README-CFG.txt for help on options
    # theme
    theme = GreyMatter
    # gui
    gui = start
    gui_transition = fade
    gui_style = flow
    gui_rows = 2
    # device
    device = usb
    ntfs_write = 1
    # language related options:
    # translation = XX
    # db_language = XX
    # this is required for asian languages:
    # load_unifont = 1
    # NAND Emulation (wiiware/VC)
    nand_emu_path = usb:/nand
    # Return to loader
    return_to_channel = UCXF
    # Multiple profile filter config
    profile_names = sample1, sample2
    save_filter = 1
    # GC memory card emulation
    mem_card_emu = 1
    mem_card_size = 2
    # Nintendont 
    nintendont_config_mode = arg
    update_nintendont = 1

## 샘플 titles.txt 파일

	RFNP = Wii Fit
	RHAP = Wii Play
	RSPP = Wii Sports
	RMGP = Super Mario Galaxy

