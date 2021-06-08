# web3-react-sample

Web3jsProvider.tsx
- redux, react-route처럼 앱 전체를 감싸는 파일. 
- web3-react를 세팅하기 위한 기본적인 파일 같음.

connector.ts
- inject 할 네트워크의 chain id값을 들고 있고, 연결 관련 객체를 리턴해주는 파일.

Connect.tsx
- connector.ts에서 injected 객체를 받은 후 계정(지갑)에 연동(로그인)하는 파일.
- 연결에 성공했다면 children(Web3jsComponent.tsx)을 보여주고, 나머지 경우엔 연결 버튼을 보여준다.

Web3jsComponent.tsx
- 계정에 성공적으로 연결되었을 경우에 렌더링 되는 컴포넌트.
- 연동된 계정의 주소를 화면에 보여준다.