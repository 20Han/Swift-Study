# RxSwift
* subscribe가 호출되는 순간 부터 observable의 데이터들이 발행되고 가공된다. 그래서 subscribeOn을 어디에서 호출하던 가장 첫번째 operator부터 해당 스레드에서 실행된다
* side effect : observable에서 발행된 데이터가 아닌 외부의 데이터를 바꾸는 작업. (ex: 외부의 image variable에 다운받은 이미지를 설정한다.) 
* side effect는  do, subscribe에서만 가능하다.
* do : subscribe와 비슷한데 Observable을 반환한다는 점이 다름
