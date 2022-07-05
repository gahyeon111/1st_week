# First_Miracle
세 개의 탭(phone, gallery, 2048)으로 이루어진 애플리케이션입니다.
+ 원하는 연락처를 추가로 저장하고 이미지를 확대해서 볼 수 있습니다.
+ 2048 탭에서는 기존의 2048 게임을 버튼을 눌러 플레이 할 수 있습니다.
+ 이미지 추가 (첫 번째 메일)

#### 개발팀원
  + 한양대 컴퓨터소프트웨어학부 남하욱
  + KAIST 전산학부 이가현

#### 개발환경
  + OS: Android
  + Language: Kotlin
  + IDE: Android Studio
  + Target Device: Galaxy S7

## Tab1 - Phone
+ 이미지 추가
#### Major features
+ 애플리케이션 안의 json 파일의 data를 가져와 listview로 보여줍니다.
+ 메인 화면에는 저장되어 연락처의 이름만 보이며, 이름으로 정렬되어 있습니다.
  + 각각의 연락처를 누르면 상세정보(이미지, 이름, 연락처)가 적혀있는 화면이 뜹니다.
    + 왼쪽 상단의 뒤로가기 버튼을 통해서 다시 전 화면으로 돌아갈 수 있습니다.
+ 오른쪽 하단의 + 버튼을 통해 새로운 연락처(이름, 연락처)를 추가할 수 있습니다.
  + 이때 사진은 애플리케이션의 defalt 사진(mario)으로 추가됩니다.
  
#### 기술설명
1. ViewPager2 & Tablayout
> ViewPager2와 tablayout을 통해 3개의 탭(fragment)을 구현하였습니다. viewpager2를 각각의 fragment와 연동하여 탭을 클릭했을 때뿐만 아니라 스와이프를 통해서도 탭 전환이 가능하게 했습니다.
2. Listview
> Adapter를 이용해 데이터와 각 리스트(연락처)의 view를 연결해 listview를 구현했습니다.
3. Intent(subactivity)
> 이동할 subactivity class를 선언하고 intent를 통해 이를 호출해 subactiviy를 구현했습니다.

## Tab 2 - Gallery
+ 이미지 추가
#### Major features
+ 애플리케이션 안(drawable 폴더)의 이미지 파일의 data를 가져와 gridview로 보여줍니다.
+ 각 이미지를 클릭하면 확대된 화면이 뜨며, 한 번 더 누르며 메인 화면으로 돌아갑니다.

#### 기술설명
1. Gridview
> tab1처럼 adapter를 이용해 gridview를 구현했습니다.
2. tab1처럼 intent를 통해 subactivity를 구혔했습니다.
