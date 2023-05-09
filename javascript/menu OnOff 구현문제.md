<img width="592" alt="image" src="https://github.com/kyungkyuBae/TIL/assets/131759810/a437ea96-eccf-417f-8c4b-5b9be8130291" >

클릭하면 메뉴바가 사라지고 생기는 버튼을 만들고 있는데
이벤트리스너 내부에서

menu의 display가 none이거나 flex 일때 경우의 수를 나눠서
하면 된다고 생각

실행해보니 무반응이여서 navList.style.display 값을 console.log()로 출력해보았는데
아무것도 받아오지 못했다
왜 값을 받아오지 못할까

구글링을 해보니 자바스크립트에서 css를 주지않은것은 빈문자열을 반환한다는 것이였다
자바스크립트 내부에서 css를 주는것은 별로 좋은 해결방안이 아닌 것 같아서

window 객체 메서드인 getComputedStyle 를 사용했더니 해결되었다

<img width="857" alt="image" src="https://github.com/kyungkyuBae/TIL/assets/131759810/82b47f4c-f101-4b4b-bd77-19bc39dd54ad">
