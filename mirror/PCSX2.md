## Contents

    

1. 개요 
2. 상세 
3. 요구사항 
4. 한계 
5. [PCSX2/호환성리스트](PCSX2/%ED%98%B8%ED%99%98%EC%84%B1%EB%A6%AC%EC%8A%A4%ED%8A%B8.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/PCSX2?action=edit&section=1)]

# 1. 개요 ¶

[플레이스테이션2](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98%202.md)
소프트를 돌릴 수 있는 PC용
[에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md)이다.
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)이며 라이센스는 GPL.

  

[공식 홈페이지](http://pcsx2.net/)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PCSX2?action=edit&section=2)]

# 2. 상세 ¶

PS1 에뮬레이터와 비슷하다. 퀄리티도 완성된 PS1 버전에 근접할 정도로 훌륭하다. 다만 여타 에뮬레이터와 같이 법망을 피하기 위해 몇가지
불편한 수단을 취하고 있으며, 덕분에 유저가 PS2의 BIOS 를 직접 떠야 한다는 불편함이 있다.

  

2014년 6월 기준으로 최신 안정화버전은 2014년 2월 2일에 나온 1.2.1

  

1.2.1버전기준으로 2489개의 게임중에서 142개를 제외한 2347개의 게임이 시작부터 엔딩까지 볼수있다는 Playable에 속한다.

  

2013년 12월 보안업체인 AVG와 제휴를 발표했다. 개발기간이 10년을 넘어 침체에 빠져 있었는데 다시 개발에 집중할 수 있기
위해서라고. 그래서 AVG툴바가 설치 버전에 포함된다.(물론 툴바를 설치할지 말지는 선택할 수 있다. 무설치 버전도 있다.)

  

발에 채이는 [PS2](PS2.md)를 냅두고 끝을 모르는 요구사항을 필요로 하는 PC 에뮬을 즐기겠다는 것이 멍청하게 보일수도
있지만, 3D 에뮬레이터 특성상 엄청난 비주얼 향상이라는 장점이 있기 때문에 원활히 플레이하는 걸 고대하는 유저들도 꽤 있다. 일단, 그래픽
자체를 PS2 의 512x384 가 아니라 1920x1080 같은 엄청난 고해상도로 렌더링 할 수 있어서 계단현상등 화질이 훨씬 깨끗하며,
여기에 유저들이 만든 그래픽패치로 [PS3](PS3.md)보다 뛰어난 그래픽(...)으로 플레이 할 수 있기 때문. 물론 PS2 와
비슷한 스펙(640x480)으로 맞추고 게임하면 지금도 아주 잘 돌아간다. <del>하지만 거기에 산이 있으니까 오르는 거지</del> 물론
그래픽만 향상되는것도 아니다. 로딩역시 향상되며 특히 SSD로 구동할 경우 미칠듯한 로딩속도로 이것때문에 까였던 부분이 날개를 달아준다고
해도 될 정도. 그 외 본체에서 8MB라는 초월적으로 적은 메모리 카드의 용량의 신경을 쓸 필요도 없으며 액플이나 강제세이브가 자유로운
여러장점이 있다.

  

차라리 [플레이스테이션3](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%983.md)로 돌리자는 의견이 있지만, 최신 플스3은 플스2 호환 기능이 제거되었으며 그나마도 구버전 플스3에서도 플스2 게임은 완벽하게
호환이 안 된다.만약 PS3 가 자체 성능만으로 PS2 게임을 돌리는 게 가능했더라면 HD컨버전이라는 핑계로 PS3 에 최적화해서 다시
개발한 [갓 오브 워](%EA%B0%93%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C.md) 콜렉션이나 [슬라이쿠퍼](%EC%8A%AC%EB%9D%BC%EC%9D%B4%20%EC%BF%A0%ED%8D%BC.md) 콜렉션 등은 나올 필요도 없었다.
`[1]` 다만 콜렉션은 와이드라는 점,3D 입체영상을 지원한다는 점,트로피 대응된다는 점이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PCSX2?action=edit&section=3)]

# 3. 요구사항 ¶

다른 고전 게임기의 에뮬레이터가 사양이 매우 낮고, 대부분 CPU 만으로 에뮬을 돌리는데 반해 PS2 는 지포스2 수준의 3D 를 지원하는
게임기라 CPU와 GPU 전부 높은 사양을 필요로 한다. 3D는 2D와 달리 해상도를 올리면 계단현상 등이 완화되고 더 나은 화질을 기대할
수 있기 때문에 단지 실기 그대로 에뮬하는 것만이 아니라 화질을 더 올려야 하는 필요가 있기 때문이다. 덕분에 현존 에뮬레이터 중 가장 최신
PC 기술까지 사용한다. 실기해상도 640x512 수준이라면 이미 현재 사양으로도 떡치고도 남는다.

  

현재 r5029 까지 오면서 지원하는 PC 옵션은 아래와 같다.

  

  * 쿼드코어(4 CPU)까지 지원
  * x86 SSE 2/3/4 추가명령어`[2]`
  * 인텔 AVX 추가명령어`[3]`
  * [nVIDIA](nVIDIA.md) GPU`[4]`
  * [DirectX](DirectX.md)9/11`[5]`  

이에 따르면 최소사양은 적어도 SSE 2 이상을 지원하는 CPU 에 DirectX 9 이상을 지원하는 그래픽이 필요하다는 말이 된다. 물론
이는 개꿈이고 실제로는 PS2 초기의 2D 위주의 저사양(?) 게임을 대충 돌리는데에만 듀얼코어 2.5 Ghz 이상에 nVIDIA
6600GT 이상의 카드가 필요하다.

  

만약 고해상도로 마음껏 돌리고자 한다면 AVX 명령어를 지원하는 쿼드코어 CPU 인 인텔 i5-2500K 이상에 4 Ghz 이상으로
오버클럭, nVIDIA GTX570 이상으로 장착하는 것이 최선이다. (SLI 는 미지원) 이 사양을 갖추면 네이티브 해상도 4x
(640x480 -> 2560x1920)으로 엄청나게 깔끔한 화면으로 플레이 할 수 있다. 심지어 사운드 싱크가 매우 중요한 [비트매니아IIDX](%EB%B9%84%ED%8A%B8%EB%A7%A4%EB%8B%88%EC%95%84%20IIDX.md)같은 물건도 살짝만
적응하면 쓸만한 수준으로 플레이가 가능해진다. 단, ZOE 아누비스나 갓오브워 같은 극한의 3D 사양을 필요로 하는 일부 게임은 여전히 30
fps 까지 내려간다. 이럴 땐 2x 정도로만 해도 프레임드랍 없이 잘 돌아간다.

  

쿼드코어까지 지원하는 현재로선 CPU 보단 GPU 에 병목이 집중된 상황이므로 차세대 GPU 가 나오면 Native x4 해상도로도 원활히
돌아갈 가능성이 높다. 아니면 x2 로만 낮춰도 풀프레임으로 플레이 할 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PCSX2?action=edit&section=4)]

# 4. 한계 ¶

성능으로는 거의 극복해낸 PCSX2 의 최대 장애물은 게임 호환성이다. 한때 비디오 게임시장을 완전히 장악했던 만큼 발매한 타이틀이
수천개이고 개중엔 잘 안쓰는 요상한 코드까지 활용한 게임들도 많다. 거의 버그 같은 테크닉을 사용할 때도 있으며, 이는 에뮬레이터 개발의
장애물이 된다. [파이널 판타지10](%ED%8C%8C%EC%9D%B4%EB%84%90%20%ED%8C%90%ED%83%80%EC%A7%80%2010.md) 같은
초유명작의 경우 매우 활발하게 보완이 이뤄지고 있기 때문에 사실상 99% 수준으로 플레이가 가능하지만 마이너한 작으로 갈수록 구동조차
불가능한 경우가 대다수다. 그리고 어째서인지 구버전에서는 완벽구동 되던 작품들이 최신버전와서는 타이틀화면에서 프리징이 걸려 진행을 못하는
작품들도 있다.`[6]` 그래도 버전업을 하면서 꾸준히 개선되고 있으므로 기다려보자. 플레이하기 전에 PCSX2 공식 홈페이지의 호환성
차트를 확인하고, 실제 세팅은 구글로 검색하면 된다.

  

2013년 5월, 플2가 발표된지 약 13년이 지난 지금도 에뮬의 완성도는 높지만 실질적인 완벽 구동률은 낮다. 차라리 게임큐브, 위의
에뮬인 돌핀이 훨씬 안정적인 모습을 보여준다. 여타 사이트에서 pcsx2를 돌려본 유저들이 그래픽 칭송을 하지만 속지 말자. 대부분의
게임들이 완벽구동+어느 정도 구동 이런 구성이다. 그외 불안정하고 미완성적인 모습들이 너무 많다.

  

만약 CPU나 GPU가 떨어진다면 내장된 스피드핵 같은 걸로 프레임스킵을 해보자. 게임에 따라 사양이 낮으면 문제가 없기도 한다.

  

[비트매니아](%EB%B9%84%ED%8A%B8%EB%A7%A4%EB%8B%88%EC%95%84.md) 같이 음성싱크가 중요한 경우에는
사운드 플러그인에서 가장 레이턴시가 낮은 세팅으로 맞추면 실기와 거의 유사해진다. 단, 이 경우에는 CPU 성능이 중요해진다.

  

치트 코드 기능은 cheats 폴더에 게임의 코드명으로 된 .pnach 형식의 텍스트 파일`[7]`에 형식에 맞게 RAW코드로 변환된 액션
리플레이 코드를 넣으면 된다. [치트오매틱](%EC%B9%98%ED%8A%B8%EC%98%A4%EB%A7%A4%ED%8B%B1.md)
등의 PC용 에디터 프로그램도 아주 간단히 먹힌다. PS2 실기와 세이브데이터를 교환할 수도 있다. elf파일 형태의 코드브레이커도
지원되지만 번거로워서 쓸 일이 없다.

  

r5011 부터 기존에 2D 텍스쳐의 테두리에 보이던 지저분한 스프라이트들이 사라졌다! 이제 화질면으로는 실기와 완벽히 동일한 상태다. 단,
아직 3D 오브젝트에서 가려져야 할 부분이 전면에 나오는 경우가 종종 있고 광원 효과가 깨진다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PCSX2?action=edit&section=5)]

# 5. [PCSX2/호환성리스트](PCSX2/%ED%98%B8%ED%99%98%EC%84%B1%EB%A6%AC%EC%8A%A4%ED%8A%B8.md) ¶

  

`\----`

  * `[1]` 최초기형 20G/60G 버전은 98%, 그 다음에 나온 초기 80G 는 50% 가량. 그나마도 '업스케일' 한 수준이라 PC 에뮬과는 격이 다르다.
  * `[2]` CPU 세대마다 지원버전 수준이 차이가 난다
  * `[3]` 샌디브릿지 CPU 부터 추가되었으며, CPU-Z 등으로 확인 가능하다
  * `[4]` 개발 자체가 nVIDIA 6600GT 이상을 타겟으로 하고 있다. [AMD](AMD.md)는 아예 에러가 나기도 한다.
  * `[5]` DX11 이 화질이 더 나은 건 아니지만 추가명령어를 사용하여 속도가 더 빠르다.
  * `[6]` GTA시리즈나 YS6, 미연시 외 몇몇 작품들
  * `[7]` 예를 들어 캡틴 츠바사(...)의 코드명은 2CF3EFF3. 콘솔창에서 확인 가능하며, 강제세이브 파일명 괄호안 부분과 똑같다.
