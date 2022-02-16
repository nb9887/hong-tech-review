# hong-tech-review

※본 자료는 우아한형제들 김영한 개발리드팀장님의 강의에서 발췌하였습니다.

스프링을 배워야 하는 이유?
스프링은 좋은 객체 지향 애플리케이션을 개발할 수 있게 도와주는 Framework

- 좋은 객체 지향 설계의 5가지 원칙 (SOLID)

SRP (Single Responsibility Principle) : 단일 책임 원칙 
- 한 클래스는 하나의 책임만 가져야 한다.
- 하나의 책임이라는 것은 모호하다.

OCP (Open/closed principle) 개방 폐쇄 원칙
확장에는 열려 있으나, 변경에는 닫혀 있어야 한다.

LSP 리스코프 치환 원칙(Liskov substitution principle)
프로그램의 객체는 프로그램의 정확성을 깨뜨리지 않으면서, 하위 타입의 인스턴스로 바꿀 수 있어야 한다.
ex. 자동차 인터페이스 '엑셀'은 앞으로 가라는 기능, 뒤로 가게 구현하면 LSP 위반, 느리더라도 앞으로 가야함

ISP (Interface segregation principle) 인터페이스 분리원칙
특정 클라이언트를 위한 인터페이스 여러 개가 범용 인터페이스 하나보다 낫다.
자동차/사용자를 위한 인터페이스 설계는 분리되어야 함.

DIP (Dependency inversion principle) 의존관계 역전 원칙
클라이언트 코드가 구현 클래스를 바라보지 말고, 인터페이스만 바라봄
추상화에 의존해야지 구체화에 의존하면 안됨

인터페이스를 도입하면 추상화라는 비용 발생

확장가능성이 없다
-> 바로 구현

확장가능성 있다
-> 인터페이스 구현




- [스프링을 배워야 하는 이유] - HTML enhanced for web apps!
- [좋은 객체 지향 설계의 5가지 원칙 (SOLID)] - awesome web-based text editor
- [markdown-it] - Markdown parser done right. Fast and easy to extend.
- [Twitter Bootstrap] - great UI boilerplate for modern web apps
- [node.js] - evented I/O for the backend
- [Express] - fast node.js network app framework [@tjholowaychuk]
- [Gulp] - the streaming build system
- [Breakdance](https://breakdance.github.io/breakdance/) - HTML


```sh
cd dillinger
docker build -t <youruser>/dillinger:${package.json.version} .
```

This will create the dillinger image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual
version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --cap-add=SYS_ADMIN --name=dillinger <youruser>/dillinger:${package.json.version}
```

> Note: `--capt-add=SYS-ADMIN` is required for PDF rendering.

Verify the deployment by navigating to your server address in
your preferred browser.

```sh
127.0.0.1:8000
```

## License

인프런 김영한님



