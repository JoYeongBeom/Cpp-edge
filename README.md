# Cpp-edge

1.  Visual Studio를 실행하고 새로운 프로젝트를 생성하거나 기존 프로젝트 열기,  프로젝트에 대해 우클릭하여 "속성(Properties)"을 선택

2.  C/C++ -> 일반 -> 추가 포함 디렉터리
- 설치된 OpenCV 폴더 내의 `include` 디렉터리 경로를 추가합니다.
    예: `C:\opencv\build\include`
   ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/11ea2db6-11df-482d-941a-5e8be9afa4dd)
   ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/8c844df6-589d-4fe3-9480-8c9301322ffb)
  
3. 링커 → 일반 → 추가 라이브러리 디렉터리(Additional Library Directories)
  - 빌드 환경에 맞는 lib 폴더 경로를 추가
    예: `C:\opencv\build\x64\vc16\lib` (64비트 환경일 경우)
    ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/1645edad-acc2-46e4-b280-1de8aea1a831)
    ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/d7c2d6a2-1d5e-46e4-b29d-c88b7e6c131c)

4. 링커 → 입력 → 추가 종속성(Additional Dependencies)
  - 사용하려는 OpenCV 모듈에 맞는 .lib 파일들을 추가
    (opencv_world490d.lib 디버그 모드에서는 'd' 접미사가 붙은 라이브러리 사용)
   ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/24ccb123-8a04-4737-9306-1693b4519c05)
   ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/cec812ca-5b24-40d6-9e9d-5726750a7c96)

5. 명령행 매개변수를 설정
프로젝트속성>구성속성>디버깅>명령인수
   ![image](https://github.com/JoYeongBeom/Cpp-edge/assets/127731008/9c52184c-31ac-4913-a772-8a32d13b32dd)

6. 빌드 및 실행
- 오류: opencv_world490d.dll 을 현재 프로젝트 폴더에 복사하기
- 솔루션을 빌드하고 실행하여 설정이 올바르게 되었는지 확인

