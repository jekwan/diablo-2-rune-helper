# diablo-2-rune-helper

## 요구사항 정의서

**[보러가기](https://github.com/jekwan/diablo-2-rune-helper/blob/master/SRS.md)** -> 작업 중입니다.

## 사용한 기술 스택

| 기술 | 이유 |
| :-- | :-- |
| `React` | `diablo-2-rune-helper`는 `SPA`로 구현할 예정입니다. 개발 편의를 위해 라이브러리나 프레임워크를 사용하기로 하였고, 후보군으로 `React`와 `Vue`를 생각하고 있었습니다. `Vue`는 간단한 프로젝트를 진행할 수준은 되었지만 `React`는 튜토리얼을 해본 정도이기 때문에 이 둘의 차이를 잘 모르는 상태입니다. 이 상태에서 벗어나기 위해 `React`를 사용하기로 결정하였습니다. |
| `Babel` | 최신 사양의 자바스크립트 문법과 JSX 사용을 위해 `Babel`을 사용하였습니다. `Babel`변환을 `Webpack`에서 자동으로 수행하도록 설정하였습니다. |
| `Webpack` | `plugin`, `loader` 등의 편의 기능과 더불어 `webpack-dev-server`를 사용하여 `개발-빌드-테스트`를 편하게 하기 위하여 번들링 툴로 `Webpack`을 사용하였습니다. |

## Atomic Deisgn

> [atomic-web-design](https://bradfrost.com/blog/post/atomic-web-design/)

`React`나 `Vue`와 같은 컴포넌트 기반 개발을 할 때 저는 항상 하나의 컴포넌트가 어느정도의 역할을 담당해야할지 고민했습니다. 기능에만 신경쓰다가 재사용 불가능한 거대 컴포넌트를 만들기 일쑤였습니다.  
그러던 중 `Atomic Design`을 발견했습니다. 마치 유기물을 이루는 원소를 구성하듯 웹을 이루는 컴포넌트를 구성하는 방식이 재미있어 보였습니다. 이 프로젝트에서 직접 `Atomic Design`을 공부하고 적용해봄으로써 어떤 부분이 좋고 어떤 부분이 아쉬운 지 학습해보고자 합니다.

## styled-components

`vue`는 `SFC`를 사용하면 `CSS-in-JS`방식로 컴포넌트 스타일링이 가능했습니다. 프로젝트 구조도 간단해지고 컴포넌트와 스타일간의 관계가 직관적으로 보인다는 점 덕분에 편하게 개발할 수 있었습니다.

`React`도 다양한 스타일링 방식을 지원하지만 위에서 서술한 개인적 선호에 따라 `CSS-in-JS`방식을 사용하기로 결정했습니다.

`emotion`과 `styled-components`는 큰 차이가 없어보이기도 하고, 작년(2021년)기준 `styled-components`가 2배 이상 많이 사용되고 있기 때문에 `styled-components`를 사용해 보기로 하였습니다.

> https://2021.stateofcss.com/en-US/technologies/css-in-js/

## Typescript

미정

## 상태 관리

미정
